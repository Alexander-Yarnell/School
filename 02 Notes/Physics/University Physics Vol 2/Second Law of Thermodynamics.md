---
aliases: [Ch. 4 The Second Law of Thermodynamics, Second Law, Entropy, Heat Engines, Carnot Cycle]
tags: [physics, thermodynamics, up-vol2]
unit: Thermodynamics
chapter: 4
---
# The Second Law of Thermodynamics

> [!info] [[University Physics Vol 2]] › Unit 1 — Thermodynamics › Chapter 4
> ← [[First Law of Thermodynamics]] · Next unit: [[Electric Charges and Fields]] →

**The Second Law of Thermodynamics** describes the one-way direction of natural processes. It limits how efficient engines can be and introduces **entropy**.

## Key Equations

> [!equation]
> $$e = \frac{W}{Q_h} = 1 - \frac{Q_c}{Q_h}$$
> $$K_R = \frac{Q_c}{W} \qquad K_P = \frac{Q_h}{W}$$
> $$e_{\text{Carnot}} = 1 - \frac{T_c}{T_h}$$
> $$\Delta S = \int \frac{dQ_{\text{rev}}}{T}$$
> $$S = k_B \ln W$$

---

## Reversible and Irreversible Processes
Real processes — friction, free expansion, heat flowing across a finite temperature difference — are **irreversible**. **Reversible** processes are idealized limits.

## Heat Engines
A heat engine absorbs heat $Q_h$ from a hot reservoir, does work $W$, and rejects heat $Q_c$ to a cold one. Its efficiency is always less than 1:

> [!equation]
> $$e = \frac{W}{Q_h} = 1 - \frac{Q_c}{Q_h}$$

> [!note] Connection
> Engines run on cyclic processes, for which $\Delta U = 0$ — see [[First Law of Thermodynamics]].

## Refrigerators and Heat Pumps
These use work to move heat from cold to hot. Performance is measured by the **coefficient of performance**:

> [!equation]
> $$K_R = \frac{Q_c}{W} \qquad K_P = \frac{Q_h}{W}$$

## Statements of the Second Law
- **Kelvin statement:** no engine converts heat entirely into work.
- **Clausius statement:** heat does not flow spontaneously from cold to hot.

The two statements are equivalent.

> [!note] Connection
> The Clausius statement is about the direction of heat transfer described in [[Temperature and Heat]].

## The Carnot Cycle
The **Carnot cycle** consists of two isotherms and two adiabats. It is the most efficient engine possible operating between two reservoirs:

> [!equation]
> $$e_{\text{Carnot}} = 1 - \frac{T_c}{T_h}$$

> [!note] Connection
> Isothermal and adiabatic processes are defined in [[First Law of Thermodynamics]].

## Entropy
Macroscopically, entropy change is

> [!equation]
> $$\Delta S = \int \frac{dQ_{\text{rev}}}{T}$$

The total entropy of an isolated system never decreases. Microscopically,

> [!equation]
> $$S = k_B \ln W$$

where $W$ counts the microstates. Entropy measures disorder and fixes the direction of time.

> [!warning] Notation
> In $S = k_B \ln W$, $W$ is the number of microstates — not work.

> [!note] Connection
> $k_B$ is Boltzmann's constant from the [[Kinetic Theory of Gases]].

## The Third Law
Absolute zero cannot be reached.

## See Also
- [[Temperature and Heat]]
- [[Kinetic Theory of Gases]]
- [[First Law of Thermodynamics]]

## Sources
- [University Physics Volume 2 — OpenStax](https://openstax.org/details/books/university-physics-volume-2)
- [Volume 2 table of contents (UPI library record)](https://oalib-perpustakaan.upi.edu/Record/OTLid0000379/TOC?print=1)
