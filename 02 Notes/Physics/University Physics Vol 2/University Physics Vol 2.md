---
aliases: [UP Vol 2, University Physics Volume 2, OpenStax Physics Vol 2]
tags: [physics, openstax, index]
---
# University Physics Volume 2

*University Physics* is a free, three-volume, calculus-based physics series by Samuel J. Ling, William Moebs and Jeff Sanny, published by OpenStax (Rice University). **Volume 2** has two units and 16 chapters: four on heat and energy (**Thermodynamics**), and twelve that build from static charge up to electromagnetic waves (**Electricity and Magnetism**).

> [!tip] How to read these notes
> The important equations to know and use are in pink **equation** boxes. Every chapter page lists its key equations at the top, then repeats each one in the notes where it comes up.
> The boxes turn pink once the `pink-equations` CSS snippet is switched on (Settings → Appearance → CSS snippets).

---

## Key Equations

### Thermodynamics

> [!equation] [[Temperature and Heat]]
> - Kelvin scale: $\displaystyle T(\text{K}) = T(^\circ\text{C}) + 273.15$
> - Linear expansion: $\displaystyle \Delta L = \alpha L\,\Delta T$
> - Specific heat: $\displaystyle Q = mc\,\Delta T$
> - Latent heat: $\displaystyle Q = mL$
> - Radiation (Stefan-Boltzmann): $\displaystyle P_{\text{rad}} = \sigma e A T^4$

> [!equation] [[Kinetic Theory of Gases]]
> - Ideal gas law: $\displaystyle pV = nRT = Nk_BT$
> - Average kinetic energy per molecule: $\displaystyle \bar{K} = \tfrac{3}{2}k_B T$
> - RMS speed: $\displaystyle v_{\text{rms}} = \sqrt{\frac{3k_B T}{m}}$

> [!equation] [[First Law of Thermodynamics]]
> - First law: $\displaystyle \Delta U = Q - W$
> - Work: $\displaystyle W = \int p\,dV$
> - Heat capacities: $\displaystyle C_p = C_v + R$
> - Adiabatic process: $\displaystyle pV^{\gamma} = \text{const}, \quad \gamma = C_p/C_v$

> [!equation] [[Second Law of Thermodynamics]]
> - Engine efficiency: $\displaystyle e = \frac{W}{Q_h} = 1 - \frac{Q_c}{Q_h}$
> - Carnot efficiency: $\displaystyle e_{\text{Carnot}} = 1 - \frac{T_c}{T_h}$
> - Entropy change: $\displaystyle \Delta S = \int \frac{dQ_{\text{rev}}}{T}$
> - Microscopic entropy: $\displaystyle S = k_B \ln W$

### Electricity and Magnetism

> [!equation] [[Electric Charges and Fields]]
> - Coulomb's law: $\displaystyle F = k\frac{|q_1 q_2|}{r^2}$
> - Electric field: $\displaystyle \vec{E} = \frac{\vec{F}}{q}$
> - Dipole torque: $\displaystyle \vec{\tau} = \vec{p} \times \vec{E}$

> [!equation] [[Gauss's Law]]
> - Gauss's law: $\displaystyle \oint \vec{E}\cdot d\vec{A} = \frac{q_{\text{enc}}}{\varepsilon_0}$

> [!equation] [[Electric Potential]]
> - Point-charge potential: $\displaystyle V = k\frac{q}{r}$
> - Potential difference: $\displaystyle \Delta V = -\int \vec{E}\cdot d\vec{l}$
> - Field from potential: $\displaystyle \vec{E} = -\nabla V$

> [!equation] [[Capacitance]]
> - Capacitance: $\displaystyle C = \frac{Q}{V}$
> - Parallel plates: $\displaystyle C = \frac{\varepsilon_0 A}{d}$
> - Stored energy: $\displaystyle U = \tfrac{1}{2}CV^2$
> - Electric energy density: $\displaystyle u_E = \tfrac{1}{2}\varepsilon_0 E^2$

> [!equation] [[Current and Resistance]]
> - Current: $\displaystyle I = \frac{dQ}{dt}$
> - Resistance: $\displaystyle R = \rho\frac{L}{A}$
> - Ohm's law: $\displaystyle V = IR$
> - Power: $\displaystyle P = IV = I^2R = \frac{V^2}{R}$

> [!equation] [[Direct-Current Circuits]]
> - Series resistors: $\displaystyle R_s = R_1 + R_2 + \cdots$
> - Parallel resistors: $\displaystyle \frac{1}{R_p} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots$
> - Charging capacitor: $\displaystyle q(t) = C\varepsilon\left(1 - e^{-t/RC}\right)$

> [!equation] [[Magnetic Forces and Fields]]
> - Force on a moving charge: $\displaystyle \vec{F} = q\vec{v}\times\vec{B}$
> - Radius of circular motion: $\displaystyle r = \frac{mv}{qB}$
> - Force on a wire: $\displaystyle \vec{F} = I\vec{L}\times\vec{B}$
> - Torque on a loop: $\displaystyle \vec{\tau} = \vec{\mu}\times\vec{B}$

> [!equation] [[Sources of Magnetic Fields]]
> - Biot-Savart law: $\displaystyle d\vec{B} = \frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{r^2}$
> - Ampère's law: $\displaystyle \oint \vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}}$
> - Straight wire: $\displaystyle B = \frac{\mu_0 I}{2\pi r}$

> [!equation] [[Electromagnetic Induction]]
> - Faraday's law: $\displaystyle \varepsilon = -N\frac{d\Phi_B}{dt}$
> - Motional emf: $\displaystyle \varepsilon = Blv$
> - Induced electric field: $\displaystyle \oint \vec{E}\cdot d\vec{l} = -\frac{d\Phi_B}{dt}$

> [!equation] [[Inductance]]
> - Self-induced emf: $\displaystyle \varepsilon = -L\frac{dI}{dt}$
> - Stored energy: $\displaystyle U = \tfrac{1}{2}LI^2$
> - RL time constant: $\displaystyle \tau_{RL} = \frac{L}{R}$
> - LC frequency: $\displaystyle \omega_0 = \frac{1}{\sqrt{LC}}$

> [!equation] [[Alternating-Current Circuits]]
> - Impedance: $\displaystyle Z = \sqrt{R^2 + (X_L - X_C)^2}$
> - Average power: $\displaystyle P_{\text{avg}} = I_{\text{rms}}V_{\text{rms}}\cos\phi$
> - Transformer: $\displaystyle \frac{V_s}{V_p} = \frac{N_s}{N_p}$

> [!equation] [[Electromagnetic Waves]]
> - Ampère-Maxwell law: $\displaystyle \oint \vec{B}\cdot d\vec{l} = \mu_0 I + \mu_0\varepsilon_0\frac{d\Phi_E}{dt}$
> - Speed of light: $\displaystyle c = \frac{1}{\sqrt{\mu_0\varepsilon_0}}$
> - Poynting vector: $\displaystyle \vec{S} = \frac{1}{\mu_0}\vec{E}\times\vec{B}$

---

## Unit 1 — Thermodynamics

How heat, temperature, work and energy relate, from single molecules to engines. Its core results are energy conservation (the first law) and the one-way direction of natural processes (the second law).

1. [[Temperature and Heat]] — thermal equilibrium and the zeroth law; thermometers and scales; thermal expansion; specific heat and calorimetry; phase changes and latent heat; conduction, convection, radiation.
2. [[Kinetic Theory of Gases]] — ideal gas law; pressure and temperature explained by molecular motion; rms speed; equipartition and heat capacity; Maxwell-Boltzmann speed distribution.
3. [[First Law of Thermodynamics]] — systems; work, heat and internal energy; ΔU = Q − W; isothermal, isobaric, isochoric, adiabatic processes; Cv and Cp of an ideal gas.
4. [[Second Law of Thermodynamics]] — reversible vs irreversible processes; heat engines; refrigerators and heat pumps; Kelvin and Clausius statements; Carnot cycle; entropy.

## Unit 2 — Electricity and Magnetism

Charges and the fields they make, circuits, magnetism, and how changing fields create each other — ending with Maxwell's equations showing that light is an electromagnetic wave.

5. [[Electric Charges and Fields]] — charge and its conservation; conductors, insulators, induction; Coulomb's law; electric field; continuous distributions; field lines; dipoles.
6. [[Gauss's Law]] — electric flux; Gauss's law; using symmetry; conductors in electrostatic equilibrium.
7. [[Electric Potential]] — potential energy; potential and voltage; E = −∇V; equipotentials; applications.
8. [[Capacitance]] — C = Q/V; series and parallel; stored energy; dielectrics.
9. [[Current and Resistance]] — current and drift velocity; resistivity; Ohm's law; electrical power; superconductors.
10. [[Direct-Current Circuits]] — emf and internal resistance; resistor combinations; Kirchhoff's rules; meters; RC circuits; household safety.
11. [[Magnetic Forces and Fields]] — force on moving charges and wires; circular motion; torque on loops; Hall effect; mass spectrometer, cyclotron.
12. [[Sources of Magnetic Fields]] — Biot-Savart law; wires and loops; parallel currents; Ampère's law; solenoids and toroids; magnetism in matter.
13. [[Electromagnetic Induction]] — Faraday's and Lenz's laws; motional emf; induced electric fields; eddy currents; generators and back emf.
14. [[Inductance]] — mutual and self-inductance; magnetic energy; RL, LC and RLC circuits.
15. [[Alternating-Current Circuits]] — reactance and impedance; AC power and rms values; resonance; transformers.
16. [[Electromagnetic Waves]] — Maxwell's equations and displacement current; plane waves; Poynting vector; radiation pressure; the electromagnetic spectrum.

## The Other Volumes

- [[University Physics Vol 1]] — mechanics (Ch. 1–14) and waves and acoustics (Ch. 15–17: oscillations, waves, sound).
- [[University Physics Vol 3]] — optics (Ch. 1–4: nature of light, geometric optics, interference, diffraction) and modern physics (Ch. 5–11).

Read Volume 2 free online starting at [Chapter 1](https://openstax.org/books/university-physics-volume-2/pages/1-introduction).

## Your Notes
- [[Electro Magnatism]] — your Engineering Physics 2 overview of Unit 2
- [[Coulombs Law]] · [[Guasess law]]

## Sources
- [University Physics Volume 1 — OpenStax](https://openstax.org/details/books/university-physics-volume-1)
- [University Physics Volume 2 — OpenStax](https://openstax.org/details/books/university-physics-volume-2)
- [University Physics Volume 3 — OpenStax](https://openstax.org/details/books/university-physics-volume-3)
- [Volume 2, Chapter 1 introduction and outline](https://openstax.org/books/university-physics-volume-2/pages/1-introduction)
- [Volume 2 table of contents (UPI library record)](https://oalib-perpustakaan.upi.edu/Record/OTLid0000379/TOC?print=1)
