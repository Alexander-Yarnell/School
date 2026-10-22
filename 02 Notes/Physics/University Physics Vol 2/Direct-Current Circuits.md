---
aliases: [Ch. 10 Direct-Current Circuits, DC Circuits, Kirchhoff's Rules, RC Circuits, EMF]
tags: [physics, electromagnetism, circuits, up-vol2]
unit: Electricity and Magnetism
chapter: 10
---
# Direct-Current Circuits

> [!info] [[University Physics Vol 2]] › Unit 2 — Electricity and Magnetism › Chapter 10
> ← [[Current and Resistance]] · Next: [[Magnetic Forces and Fields]] →

**Direct-Current Circuits** puts sources, resistors and capacitors together and gives the tools — resistor combinations and Kirchhoff's rules — to solve any DC circuit.

## Key Equations

> [!equation]
> $$V_{\text{terminal}} = \varepsilon - Ir$$
> $$R_s = R_1 + R_2 + \cdots$$
> $$\frac{1}{R_p} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots$$
> $$\sum I_{\text{in}} = \sum I_{\text{out}} \qquad \sum_{\text{loop}} \Delta V = 0$$
> $$q(t) = C\varepsilon\left(1 - e^{-t/RC}\right), \qquad \tau = RC$$

---

## EMF and Internal Resistance
A source's **emf** $\varepsilon$ is the work per unit charge it supplies. Its **terminal voltage** drops as current flows through its internal resistance $r$:

> [!equation]
> $$V_{\text{terminal}} = \varepsilon - Ir$$

## Resistors in Series and Parallel
> [!equation]
> $$R_s = R_1 + R_2 + \cdots$$
> $$\frac{1}{R_p} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots$$

> [!tip] Compare
> Capacitors combine the opposite way — see [[Capacitance]].

## Kirchhoff's Rules
> [!equation]
> $$\sum I_{\text{in}} = \sum I_{\text{out}} \qquad \sum_{\text{loop}} \Delta V = 0$$

- **Junction rule:** current into a junction equals current out — this is **charge conservation** (see [[Electric Charges and Fields]]).
- **Loop rule:** voltages around any closed loop sum to zero — this is **energy conservation**.

Together they solve any DC circuit.

## Meters
- **Ammeters** go in **series** and have **low** resistance.
- **Voltmeters** go in **parallel** and have **high** resistance.

## RC Circuits
When a capacitor charges or discharges through a resistor, its charge rises or decays exponentially with time constant $\tau = RC$. Charging:

> [!equation]
> $$q(t) = C\varepsilon\left(1 - e^{-t/RC}\right), \qquad \tau = RC$$

> [!note] Connection
> Capacitors are covered in [[Capacitance]]. RL circuits in [[Inductance]] behave similarly, with time constant $\tau = L/R$.

## Household Wiring and Safety
Grounding, fuses, circuit breakers and GFCIs prevent shocks and fires.

## See Also
- [[Systems of Linear Equations]] (Linear Algebra)
- [[Current and Resistance]]
- [[Capacitance]]
- [[Inductance]]
- [[Alternating-Current Circuits]]

## Sources
- [University Physics Volume 2 — OpenStax](https://openstax.org/details/books/university-physics-volume-2)
- [Volume 2 table of contents (UPI library record)](https://oalib-perpustakaan.upi.edu/Record/OTLid0000379/TOC?print=1)
