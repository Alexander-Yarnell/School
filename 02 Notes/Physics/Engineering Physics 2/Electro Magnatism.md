---
banner: "![[Physics-Banner.png]]"
date: 2026-10-07
Time: 09:45:00 pm
Class: Engineering Physics 2
tags:
  - Physics
  - Electromagnetism
aliases:
  - Electromagnetism
  - EM
Book: "[[Phyics-Volume-2.pdf]]"
---
---
# Electromagnetism

> [!abstract] Overview
> **Electromagnetism** is the branch of physics that studies the **electromagnetic force**, the interaction between electrically charged particles. It is one of the four fundamental forces of nature (with gravity, the strong nuclear force and the weak nuclear force). It covers **electricity**, **magnetism** and **light**, and it shows that all three are parts of one phenomenon: the **electromagnetic field**.

**Quick facts**

| | |
|---|---|
| **Force carrier** | Photon |
| **Acts on** | Electric charge |
| **Range** | Infinite (falls off as $1/r^2$) |
| **Relative strength** | ~$10^{36}$ times stronger than gravity |
| **Governing laws** | <mark style="background: #ADCCFFA6;">Maxwell</mark>'s equations + <mark style="background: #ADCCFFA6;">Lorentz</mark> force law |
| **Key constants** | $\epsilon_0,\ \mu_0,\ c$ |

---
# Contents
- [[#History]]
- [[#Electric Charge]]
- [[#Electric Fields]]
- [[#Gauss's Law]]
- [[#Electric Potential]]
- [[#Capacitance]]
- [[#Electric Current & Circuits]]
- [[#Magnetism]]
- [[#Sources of Magnetic Fields]]
- [[#Electromagnetic Induction]]
- [[#Inductance]]
- [[#Maxwell's Equations]]
- [[#Electromagnetic Waves]]
- [[#Applications]]
- [[#Key Constants]]
- [[#Equation Sheet]]

---
# History
- **~600 BC**: <mark style="background: #ADCCFFA6;">Thales of Miletus</mark> sees that rubbed amber attracts light objects. *Electron* is the Greek word for amber.
- **1600**: <mark style="background: #ADCCFFA6;">William Gilbert</mark> publishes *De Magnete*, separating electric effects from magnetic ones, and describes the Earth as a giant magnet.
- **1785**: <mark style="background: #ADCCFFA6;">Charles-Augustin de Coulomb</mark> measures the force between charges ([[Coulombs Law]]).
- **1800**: <mark style="background: #ADCCFFA6;">Alessandro Volta</mark> builds the first battery (the voltaic pile).
- **1820**: <mark style="background: #ADCCFFA6;">Hans Christian Ørsted</mark> sees a current-carrying wire deflect a compass needle. This is the **first link between electricity and magnetism**.
- **1820s**: <mark style="background: #ADCCFFA6;">André-Marie Ampère</mark> works out the forces between currents. <mark style="background: #ADCCFFA6;">Biot</mark> and <mark style="background: #ADCCFFA6;">Savart</mark> describe the magnetic field of a current.
- **1831**: <mark style="background: #ADCCFFA6;">Michael Faraday</mark> discovers **electromagnetic induction**: a changing magnetic field produces a current.
- **1865**: <mark style="background: #ADCCFFA6;">James Clerk Maxwell</mark> combines everything into four equations and predicts electromagnetic waves travelling at the speed of light.
- **1887**: <mark style="background: #ADCCFFA6;">Heinrich Hertz</mark> produces and detects radio waves, confirming <mark style="background: #ADCCFFA6;">Maxwell</mark>'s prediction.
- **1905**: <mark style="background: #ADCCFFA6;">Einstein</mark>'s special relativity shows that electric and magnetic fields are two views of the same field.
- **1940s**: Quantum electrodynamics (QED), the quantum theory of electromagnetism, is developed by <mark style="background: #ADCCFFA6;">Feynman</mark>, <mark style="background: #ADCCFFA6;">Schwinger</mark>, <mark style="background: #ADCCFFA6;">Tomonaga</mark> and <mark style="background: #ADCCFFA6;">Dyson</mark>.

---
# Electric Charge
Charge is a basic property of matter. It comes in two types, **positive** and **negative**.
- Like charges **repel**, and opposite charges **attract**.
- Charge is **conserved**: it cannot be created or destroyed, only moved around.
- Charge is **quantized**: every charge is a whole-number multiple of the elementary charge $e$.

$$
q = ne, \qquad e = 1.602 \times 10^{-19}\ \text{C}
$$

| Particle | Charge | Mass |
|---|---|---|
| Electron | $-1.602\times10^{-19}$ C | $9.109\times10^{-31}$ kg |
| Proton | $+1.602\times10^{-19}$ C | $1.673\times10^{-27}$ kg |
| Neutron | $0$ | $1.675\times10^{-27}$ kg |

**Conductors** let charges (electrons) move freely, as in metals. **Insulators** hold charges in place, as in glass and rubber. Objects become charged by **friction**, **conduction** (contact) or **induction** (bringing a charge close without touching).

See also: [[Atomic Structures]], [[Lecture 1]]

## Coulomb's Law
The force between two point charges:
$$
\vec{F}_{12} = k\frac{q_1 q_2}{r^2}\hat{r}, \qquad k = \frac{1}{4\pi\epsilon_0} = 8.99\times10^{9}\ \frac{\text{N·m}^2}{\text{C}^2}
$$
- It is an inverse-square law, just like gravity, but it can push as well as pull.
- **Superposition**: the net force on a charge is the vector sum of the forces from every other charge.

→ Full note: [[Coulombs Law]]

---
# Electric Fields
The **electric field** $\vec{E}$ is the force per unit charge that a small positive test charge would feel at a point:
$$
\vec{E} = \frac{\vec{F}}{q_0} \qquad \left[\frac{\text{N}}{\text{C}} = \frac{\text{V}}{\text{m}}\right]
$$
Field of a point charge:
$$
\vec{E} = k\frac{q}{r^2}\hat{r}
$$

> [!tip] Field line rules
> - Lines start on **positive** charges and end on **negative** charges.
> - Closer lines mean a **stronger** field.
> - Lines never cross.
> - The field is tangent to the field line at every point.

**Continuous charge distributions:** split the object into small pieces $dq$ and integrate:
$$
\vec{E} = k\int \frac{dq}{r^2}\hat{r}, \qquad dq = \lambda\,dl = \sigma\,dA = \rho\,dV
$$

**Electric dipole:** two equal and opposite charges $\pm q$ a distance $d$ apart.
- Dipole moment: $\vec{p} = q\vec{d}$
- Torque in a field: $\vec{\tau} = \vec{p}\times\vec{E}$
- Potential energy: $U = -\vec{p}\cdot\vec{E}$

---
# Gauss's Law
**Electric flux** measures how much field passes through a surface:
$$
\Phi_E = \oint \vec{E}\cdot d\vec{A}
$$
**<mark style="background: #ADCCFFA6;">Gauss</mark>'s law** says the total flux through any closed surface depends only on the charge inside it:
$$
\oint \vec{E}\cdot d\vec{A} = \frac{Q_{enc}}{\epsilon_0}
$$

| Symmetry | Gaussian surface | Result |
|---|---|---|
| Point charge / sphere | Sphere | $E = \dfrac{kQ}{r^2}$ |
| Infinite line charge | Cylinder | $E = \dfrac{\lambda}{2\pi\epsilon_0 r}$ |
| Infinite plane | Pillbox | $E = \dfrac{\sigma}{2\epsilon_0}$ |
| Conductor surface | Pillbox | $E = \dfrac{\sigma}{\epsilon_0}$ |

> [!note] Conductors in electrostatic equilibrium
> - $E = 0$ **inside** the conductor.
> - Any excess charge sits on the **surface**.
> - The field just outside is **perpendicular** to the surface.

→ Full note: [[Guasess law]]

---
# Electric Potential
The **electric potential** $V$ is the potential energy per unit charge, measured in volts (V = J/C).
$$
\Delta V = -\int_a^b \vec{E}\cdot d\vec{l}, \qquad V_{point} = k\frac{q}{r}
$$
$$
U = qV, \qquad U_{12} = k\frac{q_1q_2}{r_{12}}
$$
Getting the field back from the potential:
$$
\vec{E} = -\nabla V \quad\Rightarrow\quad E_x = -\frac{\partial V}{\partial x}
$$
- **Equipotential surfaces** are always perpendicular to field lines.
- No work is done moving a charge along an equipotential.
- Uniform field: $V = Ed$.
- **Electron-volt:** $1\ \text{eV} = 1.602\times10^{-19}$ J.

---
# Capacitance
A **capacitor** stores charge and energy in an electric field between two conductors.
$$
C = \frac{Q}{V} \qquad [\text{F} = \text{C/V}]
$$
Parallel plate: $C = \dfrac{\epsilon_0 A}{d}$. With a dielectric: $C = \kappa C_0$.

| Combination | Formula |
|---|---|
| Series | $\dfrac{1}{C_{eq}} = \sum \dfrac{1}{C_i}$ |
| Parallel | $C_{eq} = \sum C_i$ |

Stored energy:
$$
U = \frac{1}{2}CV^2 = \frac{Q^2}{2C} = \frac{1}{2}QV, \qquad u_E = \frac{1}{2}\epsilon_0E^2
$$

---
# Electric Current & Circuits
**Current** is the rate at which charge flows:
$$
I = \frac{dQ}{dt} \qquad [\text{A} = \text{C/s}], \qquad I = nqv_dA
$$
**<mark style="background: #ADCCFFA6;">Ohm</mark>'s law & resistance:**
$$
V = IR, \qquad R = \rho\frac{L}{A}, \qquad P = IV = I^2R = \frac{V^2}{R}
$$

| Combination | Resistors | Capacitors |
|---|---|---|
| Series | $R_{eq} = \sum R_i$ | $\dfrac{1}{C_{eq}} = \sum \dfrac{1}{C_i}$ |
| Parallel | $\dfrac{1}{R_{eq}} = \sum \dfrac{1}{R_i}$ | $C_{eq} = \sum C_i$ |

**<mark style="background: #ADCCFFA6;">Kirchhoff</mark>'s rules**
1. **Junction rule** (conservation of charge): $\sum I_{in} = \sum I_{out}$
2. **Loop rule** (conservation of energy): $\sum \Delta V = 0$ around any closed loop

**RC circuits:** time constant $\tau = RC$
- Charging: $q(t) = Q\left(1 - e^{-t/RC}\right)$
- Discharging: $q(t) = Qe^{-t/RC}$

---
# Magnetism
Magnetic fields $\vec{B}$ are produced by **moving charges** (currents) and by the intrinsic spin of particles. The unit is the **tesla** (T); $1\ \text{G} = 10^{-4}$ T.
- Magnets always have a **north and south pole**. No magnetic monopole has ever been found.
- Field lines form **closed loops**, running outside the magnet from N to S.

## Magnetic Force
**On a moving charge (<mark style="background: #ADCCFFA6;">Lorentz</mark> force):**
$$
\vec{F} = q\left(\vec{E} + \vec{v}\times\vec{B}\right), \qquad |F_B| = qvB\sin\theta
$$
**On a current-carrying wire:**
$$
\vec{F} = I\vec{L}\times\vec{B}
$$
> [!tip] Right-hand rule
> Point your fingers along $\vec{v}$ (or $I$), curl them toward $\vec{B}$, and your thumb gives the force on a **positive** charge. Flip it for electrons.

- The magnetic force is always perpendicular to $\vec{v}$, so it **does no work** and cannot change a particle's speed.
- **Circular motion** in a uniform field:
$$
r = \frac{mv}{qB}, \qquad \omega_c = \frac{qB}{m}, \qquad T = \frac{2\pi m}{qB}
$$
- **Current loop:** magnetic moment $\vec{\mu} = NI\vec{A}$, torque $\vec{\tau} = \vec{\mu}\times\vec{B}$, energy $U = -\vec{\mu}\cdot\vec{B}$.
- **<mark style="background: #ADCCFFA6;">Hall</mark> effect:** charges pushed sideways in a conductor create a measurable voltage, $V_H = \dfrac{IB}{nqt}$.

---
# Sources of Magnetic Fields
**<mark style="background: #ADCCFFA6;">Biot</mark>–<mark style="background: #ADCCFFA6;">Savart</mark> law:** the field from a small piece of current
$$
d\vec{B} = \frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{r^2}
$$
**<mark style="background: #ADCCFFA6;">Ampère</mark>'s law:**
$$
\oint \vec{B}\cdot d\vec{l} = \mu_0 I_{enc}
$$

| Source | Magnetic field |
|---|---|
| Long straight wire | $B = \dfrac{\mu_0 I}{2\pi r}$ |
| Center of a circular loop | $B = \dfrac{\mu_0 I}{2R}$ |
| Solenoid (inside) | $B = \mu_0 nI$ |
| Toroid | $B = \dfrac{\mu_0 NI}{2\pi r}$ |

**Force between parallel wires:** $\dfrac{F}{L} = \dfrac{\mu_0 I_1 I_2}{2\pi d}$. Currents in the same direction attract; opposite directions repel.

**Magnetic materials:** *diamagnetic* materials are weakly repelled, *paramagnetic* materials are weakly attracted, and *ferromagnetic* materials (Fe, Ni, Co) are strongly attracted and can stay magnetized.

---
# Electromagnetic Induction
**Magnetic flux:**
$$
\Phi_B = \int \vec{B}\cdot d\vec{A} \qquad [\text{Wb} = \text{T·m}^2]
$$
**<mark style="background: #ADCCFFA6;">Faraday</mark>'s law:** a changing magnetic flux induces an EMF:
$$
\mathcal{E} = -N\frac{d\Phi_B}{dt}
$$
**<mark style="background: #ADCCFFA6;">Lenz</mark>'s law** (the minus sign): the induced current flows in the direction that **opposes the change** in flux.

You can change the flux by changing $B$, the area $A$, or the angle $\theta$:
- **Motional EMF** (a rod sliding on rails): $\mathcal{E} = BLv$
- **Generator** (a rotating coil): $\mathcal{E} = NBA\omega\sin(\omega t)$
- **Eddy currents**: induced loops of current in solid conductors, used in induction braking and heating.

---
# Inductance
An **inductor** resists changes in current.
$$
\mathcal{E}_L = -L\frac{dI}{dt} \qquad [\text{H} = \text{V·s/A}]
$$
- Solenoid: $L = \mu_0 n^2 A l$
- Mutual inductance: $\mathcal{E}_2 = -M\dfrac{dI_1}{dt}$
- Stored energy: $U = \dfrac{1}{2}LI^2$, energy density $u_B = \dfrac{B^2}{2\mu_0}$
- **RL circuit:** $\tau = L/R$, and $I(t) = \dfrac{\mathcal{E}}{R}\left(1 - e^{-t/\tau}\right)$
- **LC circuit:** oscillates at $\omega = \dfrac{1}{\sqrt{LC}}$
- **Transformer:** $\dfrac{V_s}{V_p} = \dfrac{N_s}{N_p}$

---
# Maxwell's Equations
These four equations, together with the <mark style="background: #ADCCFFA6;">Lorentz</mark> force, describe **all** of classical electromagnetism.

| Law | Integral form | Differential form | Meaning |
|---|---|---|---|
| **<mark style="background: #ADCCFFA6;">Gauss</mark> (electric)** | $\oint \vec{E}\cdot d\vec{A} = \dfrac{Q_{enc}}{\epsilon_0}$ | $\nabla\cdot\vec{E} = \dfrac{\rho}{\epsilon_0}$ | Charges create electric fields |
| **<mark style="background: #ADCCFFA6;">Gauss</mark> (magnetic)** | $\oint \vec{B}\cdot d\vec{A} = 0$ | $\nabla\cdot\vec{B} = 0$ | There are no magnetic monopoles |
| **<mark style="background: #ADCCFFA6;">Faraday</mark>** | $\oint \vec{E}\cdot d\vec{l} = -\dfrac{d\Phi_B}{dt}$ | $\nabla\times\vec{E} = -\dfrac{\partial\vec{B}}{\partial t}$ | A changing $B$ creates $E$ |
| **<mark style="background: #ADCCFFA6;">Ampère</mark>–<mark style="background: #ADCCFFA6;">Maxwell</mark>** | $\oint \vec{B}\cdot d\vec{l} = \mu_0 I_{enc} + \mu_0\epsilon_0\dfrac{d\Phi_E}{dt}$ | $\nabla\times\vec{B} = \mu_0\vec{J} + \mu_0\epsilon_0\dfrac{\partial\vec{E}}{\partial t}$ | Currents and a changing $E$ create $B$ |

> [!important] Displacement current
> <mark style="background: #ADCCFFA6;">Maxwell</mark>'s key addition was the term $\epsilon_0\dfrac{d\Phi_E}{dt}$, called the **displacement current**. It means a changing electric field makes a magnetic field, just as a changing magnetic field makes an electric field. Each field keeps regenerating the other, and that is what lets **electromagnetic waves** travel through empty space.

---
# Electromagnetic Waves
In empty space <mark style="background: #ADCCFFA6;">Maxwell</mark>'s equations become wave equations. The predicted wave speed is:
$$
c = \frac{1}{\sqrt{\mu_0\epsilon_0}} = 3.00\times10^{8}\ \text{m/s}
$$
<mark style="background: #ADCCFFA6;">Maxwell</mark> recognised this as the measured speed of light, which showed that **light is an electromagnetic wave**.

**Properties**
- $\vec{E}$ and $\vec{B}$ are perpendicular to each other and to the direction of travel (transverse waves).
- $E = cB$
- $c = f\lambda$
- They need no medium.
- **Energy flow (<mark style="background: #ADCCFFA6;">Poynting</mark> vector):** $\vec{S} = \dfrac{1}{\mu_0}\vec{E}\times\vec{B}$
- **Intensity:** $I = \dfrac{1}{2}c\epsilon_0E_0^2 = \dfrac{E_0B_0}{2\mu_0}$
- **Radiation pressure:** $p = I/c$ when absorbed, $2I/c$ when reflected.

## The Electromagnetic Spectrum
| Type | Wavelength | Example use |
|---|---|---|
| Radio | > 1 m | Broadcasting, communication |
| Microwave | 1 mm – 1 m | Cooking, radar, Wi-Fi |
| Infrared | 700 nm – 1 mm | Thermal imaging, remotes |
| **Visible** | **400 – 700 nm** | **Vision** |
| Ultraviolet | 10 – 400 nm | Sterilization, tanning |
| X-ray | 0.01 – 10 nm | Medical imaging |
| Gamma ray | < 0.01 nm | Cancer treatment, nuclear decay |

*Wavelength goes down, and frequency and photon energy ($E = hf$) go up, as you move down the table.*

---
# Applications
- **Electric motors**: force on a current loop in a magnetic field.
- **Generators**: <mark style="background: #ADCCFFA6;">Faraday</mark>'s law; mechanical energy becomes electrical energy.
- **Transformers**: mutual inductance steps AC voltages up or down for the power grid.
- **MRI**: strong magnetic fields and radio waves image the body.
- **Wireless communication**: radio, Wi-Fi, cell phones, GPS.
- **Electronics**: capacitors, inductors and resistors in every circuit.
- **Maglev trains and induction cooktops**: magnetic levitation and eddy currents.
- **Particle accelerators and mass spectrometers**: steering charges with $\vec{E}$ and $\vec{B}$.

---
# Key Constants
| Constant | Symbol | Value |
|---|---|---|
| Elementary charge | $e$ | $1.602\times10^{-19}$ C |
| <mark style="background: #ADCCFFA6;">Coulomb</mark> constant | $k$ | $8.99\times10^{9}$ N·m²/C² |
| Permittivity of free space | $\epsilon_0$ | $8.854\times10^{-12}$ C²/(N·m²) |
| Permeability of free space | $\mu_0$ | $4\pi\times10^{-7}$ T·m/A |
| Speed of light | $c$ | $2.998\times10^{8}$ m/s |
| Electron mass | $m_e$ | $9.109\times10^{-31}$ kg |
| Proton mass | $m_p$ | $1.673\times10^{-27}$ kg |

---
# Equation Sheet
<span class="daily-nav">[[Useful Equations|🧮 Useful Equations]]</span>

| Topic | Equation |
|---|---|
| <mark style="background: #ADCCFFA6;">Coulomb</mark>'s law | $F = k\dfrac{q_1q_2}{r^2}$ |
| Electric field | $\vec{E} = \vec{F}/q$ |
| <mark style="background: #ADCCFFA6;">Gauss</mark>'s law | $\oint \vec{E}\cdot d\vec{A} = Q_{enc}/\epsilon_0$ |
| Potential | $V = kq/r$, $\ \Delta V = -\int\vec{E}\cdot d\vec{l}$ |
| Capacitance | $C = Q/V$, $\ U = \tfrac{1}{2}CV^2$ |
| <mark style="background: #ADCCFFA6;">Ohm</mark>'s law | $V = IR$, $\ P = IV$ |
| <mark style="background: #ADCCFFA6;">Lorentz</mark> force | $\vec{F} = q(\vec{E} + \vec{v}\times\vec{B})$ |
| <mark style="background: #ADCCFFA6;">Biot</mark>–<mark style="background: #ADCCFFA6;">Savart</mark> | $d\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{I\,d\vec{l}\times\hat{r}}{r^2}$ |
| <mark style="background: #ADCCFFA6;">Ampère</mark>'s law | $\oint\vec{B}\cdot d\vec{l} = \mu_0 I_{enc}$ |
| <mark style="background: #ADCCFFA6;">Faraday</mark>'s law | $\mathcal{E} = -N\,d\Phi_B/dt$ |
| Inductor | $\mathcal{E} = -L\,dI/dt$, $\ U = \tfrac{1}{2}LI^2$ |
| EM waves | $c = 1/\sqrt{\mu_0\epsilon_0}$, $\ E = cB$ |

---
# Summary
Electromagnetism describes how charges create **electric fields**, how moving charges create **magnetic fields**, and how a field that changes in time creates the other kind. <mark style="background: #ADCCFFA6;">Maxwell</mark>'s four equations tie these ideas together and predict self-sustaining electromagnetic waves that travel at the speed of light, so light itself is an electromagnetic wave.

---
# References
[[Coulombs Law]] · [[Guasess law]] · [[Atomic Structures]] · [[Lecture 1]] · [[Lecture 2]] · [[Useful Equations]] · [[SI Units ( International System of Units )]]
