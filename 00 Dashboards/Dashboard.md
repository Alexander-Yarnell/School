---
banner: "![[Dashboard - banner.png]]"
content-start: 181
banner-fade: -190
banner-display: contain
banner-repeat: false
---
a---
```dataviewjs
const year = 2026;
const folderPath = "01 Journals/00 Daily Notes";
const colors = ["#3c3836", "#d65d0e", "#fe8019", "#fabd2f", "#fabd2f"];
const maxWords = 500;

dv.el("div", `**📔 Daily Notes ${year} 📔**`, { cls: "custom-heatmap-title" });

const wordCounts = {};
for (let page of dv.pages(`"${folderPath}"`)) {
  if (!/^\d{4}-\d{2}-\d{2}$/.test(page.file.name)) continue;
  const content = await dv.io.load(page.file.path);
  const body = content.replace(/^---[\s\S]*?---/, "");
  wordCounts[page.file.name] = body.trim().split(/\s+/).filter(Boolean).length;
}

function colorFor(count) {
  if (!count) return colors[0];
  const ratio = Math.min(count / maxWords, 1);
  const idx = Math.min(Math.floor(ratio * (colors.length - 1)) + 1, colors.length - 1);
  return colors[idx];
}

const start = new Date(year, 0, 1);
const end = new Date(year, 11, 31);
const startDow = start.getDay();

const days = [];
let cursor = new Date(start);
cursor.setDate(cursor.getDate() - startDow);
while (cursor <= end || cursor.getDay() !== 0) {
  days.push(new Date(cursor));
  cursor.setDate(cursor.getDate() + 1);
  if (cursor > end && cursor.getDay() === 0) break;
}

const weeks = [];
for (let i = 0; i < days.length; i += 7) {
  weeks.push(days.slice(i, i + 7));
}

const dayLabels = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];
const monthNames = ["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"];

const container = dv.el("div", "", { cls: "custom-heatmap-wrapper" });
const grid = container.createEl("div", { cls: "custom-heatmap-grid" });

// Empty corner above the day-labels column
const labelCol = grid.createEl("div", { cls: "custom-heatmap-labelcol" });
labelCol.createEl("div", { cls: "custom-heatmap-monthspacer" });
for (const label of dayLabels) {
  labelCol.createEl("div", { text: label, cls: "custom-heatmap-daylabel" });
}

// Track which months we've already labeled so each shows once
let lastMonth = -1;

for (const week of weeks) {
  const col = grid.createEl("div", { cls: "custom-heatmap-week" });

  // Find the month label for this column: use the first day in-year in this week
  const firstInYearDay = week.find(d => d.getFullYear() === year);
  let monthLabel = "";
  if (firstInYearDay) {
    const m = firstInYearDay.getMonth();
    if (m !== lastMonth) {
      monthLabel = monthNames[m];
      lastMonth = m;
    }
  }
  col.createEl("div", { text: monthLabel, cls: "custom-heatmap-monthlabel" });

  for (const day of week) {
    const dateStr = day.toISOString().slice(0, 10);
    const inYear = day.getFullYear() === year;
    const count = wordCounts[dateStr] || 0;
    const cell = col.createEl("div", { cls: "custom-heatmap-cell" });
    if (inYear) {
      cell.style.backgroundColor = colorFor(count);
      cell.setAttribute("title", `${dateStr}: ${count} words`);
    } else {
      cell.style.backgroundColor = "transparent";
    }
  }
}
```
---
```dataviewjs
const commands = app.commands.commands;

const periods = [
  { label: "📝 Daily", match: /daily/i },
  { label: "📅 Weekly", match: /weekly/i },
  { label: "🗓️ Monthly", match: /monthly/i },
  { label: "📆 Quarterly", match: /quarterly/i },
  { label: "🎯 Yearly", match: /yearly/i },
];

const container = dv.el("div", "", { cls: "daily-nav" });

for (const period of periods) {
  const cmd = Object.values(commands).find(
    c => c.id.startsWith("periodic-notes") && period.match.test(c.name)
  );

  if (cmd) {
    const link = container.createEl("a", { text: period.label, href: "#" });
    link.addEventListener("click", (e) => {
      e.preventDefault();
      app.commands.executeCommandById(cmd.id);
    });
  } else {
    container.createEl("span", {
      text: `⚠️ ${period.label} not found`,
      cls: "daily-nav-missing"
    });
  }
}
```
---
--- start-multi-column: StudyTimerRegion


```column-settings
number of columns: 2
column size: [59%, 40%]
border: off
```

```tracker
searchType: task.done
searchTarget: Studied
folder: /01 Journals/00 Daily Notes
datasetName: Studied
month:
    startWeekOn: "Sun"
    color: "#fe8019"
    showSelectedValue: true
```


--- column-end ---


```dataviewjs

const STUDY_MIN = 25;
const BREAK_MIN = 5;
const STORAGE_KEY = "studyTimerState";

function loadState() {
  const raw = localStorage.getItem(STORAGE_KEY);
  if (raw) return JSON.parse(raw);
  return {
    mode: "study",
    running: false,
    endTime: null,           // timestamp when current countdown ends, if running
    remaining: STUDY_MIN * 60, // seconds left, used when paused
    sessionCount: parseInt(localStorage.getItem("studyTimerSessions") || "0", 10),
  };
}

function saveState(state) {
  localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
}

let state = loadState();

const wrapper = dv.el("div", "", { cls: "study-timer-wrapper" });
const modeLabel = wrapper.createEl("div", { cls: "study-timer-mode" });

const radius = 90;
const circumference = 2 * Math.PI * radius;

const svgWrapper = wrapper.createEl("div", { cls: "study-timer-ring" });
svgWrapper.innerHTML = `
  <svg width="220" height="220" viewBox="0 0 220 220">
    <circle cx="110" cy="110" r="${radius}" class="study-timer-track" stroke-width="14" fill="none"/>
    <circle cx="110" cy="110" r="${radius}" class="study-timer-progress" stroke-width="14" fill="none"
      stroke-dasharray="${circumference}" stroke-dashoffset="0" transform="rotate(-90 110 110)"/>
  </svg>
`;
const progressCircle = svgWrapper.querySelector(".study-timer-progress");
const timeText = svgWrapper.createEl("div", { cls: "study-timer-time" });
const sessionText = wrapper.createEl("div", { cls: "study-timer-sessions" });

const controls = wrapper.createEl("div", { cls: "study-timer-controls" });
const startBtn = controls.createEl("button", { cls: "study-timer-btn" });
const resetBtn = controls.createEl("button", { text: "Reset", cls: "study-timer-btn" });

const modeControls = wrapper.createEl("div", { cls: "study-timer-mode-controls" });
const studyBtn = modeControls.createEl("button", { text: "Study", cls: "study-timer-mode-btn" });
const breakBtn = modeControls.createEl("button", { text: "Break", cls: "study-timer-mode-btn" });

function totalFor(mode) {
  return (mode === "study" ? STUDY_MIN : BREAK_MIN) * 60;
}

function currentRemaining() {
  if (state.running && state.endTime) {
    return Math.max(0, Math.round((state.endTime - Date.now()) / 1000));
  }
  return state.remaining;
}

function formatTime(s) {
  const m = Math.floor(s / 60).toString().padStart(2, "0");
  const sec = (s % 60).toString().padStart(2, "0");
  return `${m}:${sec}`;
}

function playChime() {
  const ctx = new (window.AudioContext || window.webkitAudioContext)();
  [440, 660].forEach((freq, i) => {
    const osc = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.frequency.value = freq;
    osc.type = "sine";
    gain.gain.setValueAtTime(0.15, ctx.currentTime + i * 0.3);
    gain.gain.exponentialRampToValueAtTime(0.001, ctx.currentTime + i * 0.3 + 0.5);
    osc.connect(gain);
    gain.connect(ctx.destination);
    osc.start(ctx.currentTime + i * 0.3);
    osc.stop(ctx.currentTime + i * 0.3 + 0.5);
  });
}

function render() {
  state = loadState(); // always read the freshest shared state
  const remaining = currentRemaining();

  // Handle countdown hitting zero, exactly once per transition
  if (state.running && remaining <= 0) {
    playChime();
    if (state.mode === "study") {
      state.sessionCount++;
      localStorage.setItem("studyTimerSessions", state.sessionCount.toString());
    }
    state.mode = state.mode === "study" ? "break" : "study";
    state.remaining = totalFor(state.mode);
    state.endTime = Date.now() + state.remaining * 1000;
    saveState(state);
  }

  const total = totalFor(state.mode);
  const shown = currentRemaining();
  timeText.setText(formatTime(shown));
  const progress = shown / total;
  progressCircle.setAttribute("stroke-dashoffset", (circumference * (1 - progress)).toString());
  modeLabel.setText(state.mode === "study" ? "STUDY" : "BREAK");
  modeLabel.style.color = state.mode === "study" ? "var(--gb-orange)" : "var(--gb-aqua)";
  progressCircle.style.stroke = state.mode === "study" ? "var(--gb-orange)" : "var(--gb-aqua)";
  studyBtn.classList.toggle("active", state.mode === "study");
  breakBtn.classList.toggle("active", state.mode === "break");
  sessionText.setText(`Sessions completed: ${state.sessionCount}`);
  startBtn.setText(state.running ? "Pause" : "Start");
}

startBtn.addEventListener("click", () => {
  state = loadState();
  if (state.running) {
    state.remaining = currentRemaining();
    state.running = false;
  } else {
    state.endTime = Date.now() + state.remaining * 1000;
    state.running = true;
  }
  saveState(state);
  render();
});

resetBtn.addEventListener("click", () => {
  state = loadState();
  state.running = false;
  state.remaining = totalFor(state.mode);
  state.endTime = null;
  saveState(state);
  render();
});

studyBtn.addEventListener("click", () => {
  state = loadState();
  state.mode = "study";
  state.running = false;
  state.remaining = totalFor("study");
  state.endTime = null;
  saveState(state);
  render();
});

breakBtn.addEventListener("click", () => {
  state = loadState();
  state.mode = "break";
  state.running = false;
  state.remaining = totalFor("break");
  state.endTime = null;
  saveState(state);
  render();
});

render();
setInterval(render, 1000);

```


--- end-multi-column


--- 
```dataviewjs
const subjects = [
    { name: "⚗️ Chemistry", folder: "02 Notes/Chemistry" },
    { name: "📐 Mathematics", folder: "02 Notes/Mathematics" },
    { name: "💻 Programming", folder: "02 Notes/Programming" },
    { name: "📘 Physics", folder: "02 Notes/Physics" }
];

const container = dv.el("div", "", { cls: "daily-nav" });

for (const subject of subjects) {

    const link = container.createEl("a", {
        text: subject.name,
        href: "#"
    });

    link.addEventListener("click", async (e) => {
        e.preventDefault();

        const date = window.moment().format("YYYY-MM-DD-HHmmss");
        const fileName = `${subject.name.replace(/[^a-zA-Z]/g, "").trim()} Note ${date}.md`;
        const filePath = `${subject.folder}/${fileName}`;

        try {
            const file = await app.vault.create(filePath, "");

            await app.workspace.getLeaf(true).openFile(file);

        } catch (err) {
            console.error(err);
            new Notice(`Could not create ${subject.name} note: ${err.message}`);
        }
    });
}
```
---
# Books
---
## Physics
![[Physics Books.base]]
## Mathematics
![[Mathematics Books.base]]
## Chemistry
![[Chemistry Books.base]]
## Programming
![[Programming Books.base]]

