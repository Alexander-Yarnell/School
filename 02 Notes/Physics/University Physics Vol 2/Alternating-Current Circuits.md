---
aliases: [Ch. 15 Alternating-Current Circuits, AC Circuits, Impedance, Reactance, Resonance, Transformers]
tags: [physics, electromagnetism, circuits, up-vol2]
unit: Electricity and Magnetism
chapter: 15
---
# Alternating-Current Circuits

> [!info] [[University Physics Vol 2]] › Unit 2 — Electricity and Magnetism › Chapter 15
> ← [[Inductance]] · Next: [[Electromagnetic Waves]] →

**Alternating-Current Circuits** covers circuits driven by sinusoidal sources: how resistors, capacitors and inductors respond, impedance, power, resonance and transformers.

## Key Equations

> [!equation]
> $$v = V_0\sin\omega t$$
> $$X_C = \frac{1}{\omega C} \qquad X_L = \omega L$$
> $$Z = \sqrt{R^2 + (X_L - X_C)^2} \qquad \tan\phi = \frac{X_L - X_C}{R}$$
> $$P_{\text{avg}} = I_{\text{rms}}V_{\text{rms}}\cos\phi \qquad \text{rms} = \frac{\text{peak}}{\sqrt{2}}$$
> $$\omega_0 = \frac{1}{\sqrt{LC}}$$
> $$\frac{V_s}{V_p} = \frac{N_s}{N_p}$$

---

## AC Sources
Voltage and current vary sinusoidally:

> [!equation]
> $$v = V_0\sin\omega t$$

> [!note] Connection
> A generator produces this kind of emf, $\varepsilon = NBA\omega\sin\omega t$ — see [[Electromagnetic Induction]].

## Simple AC Circuits
| Element | Phase of current vs voltage | Opposition |
| --- | --- | --- |
| Resistor | In phase | $R$ |
| Capacitor | Current **leads** by 90° | $X_C = 1/\omega C$ |
| Inductor | Current **lags** by 90° | $X_L = \omega L$ |

> [!equation]
> $$X_C = \frac{1}{\omega C} \qquad X_L = \omega L$$

**Phasors** are used to represent these phase relationships.

> [!note] Connection
> See [[Capacitance]] and [[Inductance]] for the components themselves.

## Series RLC Circuits
> [!equation]
> $$Z = \sqrt{R^2 + (X_L - X_C)^2} \qquad \tan\phi = \frac{X_L - X_C}{R}$$

$Z$ is the **impedance** and $\phi$ is the **phase angle**.

## Power in AC Circuits
> [!equation]
> $$P_{\text{avg}} = I_{\text{rms}}V_{\text{rms}}\cos\phi \qquad \text{rms} = \frac{\text{peak}}{\sqrt{2}}$$

## Resonance
At the resonant frequency, $X_L = X_C$, the impedance is at its minimum and the current at its maximum:

> [!equation]
> $$\omega_0 = \frac{1}{\sqrt{LC}}$$

This is the basis of **radio tuning**. The **quality factor** $Q$ measures how sharp the resonance is.

> [!note] Connection
> This is the same frequency at which an LC circuit oscillates — see [[Inductance]].

## Transformers
> [!equation]
> $$\frac{V_s}{V_p} = \frac{N_s}{N_p}$$

High-voltage transmission cuts $I^2R$ losses.

> [!note] Connection
> $I^2R$ power loss is from [[Current and Resistance]].

## See Also
- [[Inductance]]
- [[Capacitance]]
- [[Electromagnetic Induction]]
- [[Current and Resistance]]

## Sources
- [University Physics Volume 2 — OpenStax](https://openstax.org/details/books/university-physics-volume-2)
- [Volume 2 table of contents (UPI library record)](https://oalib-perpustakaan.upi.edu/Record/OTLid0000379/TOC?print=1)
