---
aliases: [Ch. 15 Oscillations, Simple Harmonic Motion, SHM, Pendulum, Damped Oscillations, Resonance]
tags: [physics, waves, up-vol1]
unit: Waves and Acoustics
chapter: 15
---
# Oscillations

> [!info] [[University Physics Vol 1]] › Unit 2 — Waves and Acoustics › Chapter 15
> ← [[Fluid Mechanics]] · Next: [[Waves]] →

**Oscillations** opens the waves unit with periodic motion — especially **simple harmonic motion (SHM)**, caused by a restoring force proportional to displacement.

## Key Equations

> [!equation]
> - **Frequency and period:** $\displaystyle f = \frac{1}{T}$
> - **Position in SHM:** $\displaystyle x(t) = A\cos(\omega t + \phi)$
> - **Velocity in SHM:** $\displaystyle v(t) = -A\omega\sin(\omega t + \phi)$
> - **Acceleration in SHM:** $\displaystyle a(t) = -A\omega^2\cos(\omega t + \phi)$
> - **Angular frequency (mass-spring):** $\displaystyle \omega = \sqrt{\frac{k}{m}}$
> - **Period (mass-spring):** $\displaystyle T = 2\pi\sqrt{\frac{m}{k}}$
> - **Total energy (mass-spring):** $\displaystyle E_{\text{Total}} = \tfrac{1}{2}kx^2 + \tfrac{1}{2}mv^2 = \tfrac{1}{2}kA^2$
> - **Speed at position x:** $\displaystyle v = \pm\sqrt{\frac{k}{m}(A^2 - x^2)}$
> - **Period (simple pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{L}{g}}$
> - **Period (physical pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{I}{mgL}}$
> - **Period (torsional pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{I}{\kappa}}$
> - **Equation of motion (damped):** $\displaystyle m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0$
> - **Underdamped solution:** $\displaystyle x(t) = A_0 e^{-\frac{b}{2m}t}\cos(\omega t + \phi)$
> - **Amplitude (forced, damped):** $\displaystyle A = \frac{F_o}{\sqrt{m^2(\omega^2 - \omega_o^2)^2 + b^2\omega^2}}$

---

## Simple Harmonic Motion
- **Period** $T$ is time per cycle; **frequency** $f = 1/T$.
- SHM happens when the restoring force grows with displacement and points back toward equilibrium.
- Amplitude $A$ is the maximum displacement.

> [!equation]
> - **Frequency and period:** $\displaystyle f = \frac{1}{T}$
> - **Position in SHM:** $\displaystyle x(t) = A\cos(\omega t + \phi)$
> - **Velocity in SHM:** $\displaystyle v(t) = -A\omega\sin(\omega t + \phi)$
> - **Acceleration in SHM:** $\displaystyle a(t) = -A\omega^2\cos(\omega t + \phi)$
> - **Angular frequency (mass-spring):** $\displaystyle \omega = \sqrt{\frac{k}{m}}$
> - **Period (mass-spring):** $\displaystyle T = 2\pi\sqrt{\frac{m}{k}}$

> [!note] Connection
> The restoring force is Hooke's law, $F = -kx$ — see [[Newton's Laws of Motion]].

## Energy in Simple Harmonic Motion
- Elastic PE is $\tfrac12 kx^2$; total energy is constant, shared between KE and PE, and equals $\tfrac12 kA^2$.

> [!equation]
> - **Total energy (mass-spring):** $\displaystyle E_{\text{Total}} = \tfrac{1}{2}kx^2 + \tfrac{1}{2}mv^2 = \tfrac{1}{2}kA^2$
> - **Speed at position x:** $\displaystyle v = \pm\sqrt{\frac{k}{m}(A^2 - x^2)}$

> [!note] Connection
> See [[Potential Energy and Conservation of Energy]]. An LC circuit is the electrical analog of a mass on a spring — [[Inductance]].

## Comparing SHM and Circular Motion
- Projecting uniform circular motion onto an axis gives simple harmonic motion.

> [!note] Connection
> Uniform circular motion is in [[Motion in Two and Three Dimensions]].

## Pendulums
- A **simple pendulum** does SHM for amplitudes below about 15°.
- **Physical** and **torsional** pendulums depend on the moment of inertia.

> [!equation]
> - **Period (simple pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{L}{g}}$
> - **Period (physical pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{I}{mgL}}$
> - **Period (torsional pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{I}{\kappa}}$

> [!note] Connection
> $I$ is from [[Fixed-Axis Rotation]].

## Damped Oscillations
- Damping forces (non-conservative) remove energy.
- **Underdamped** systems oscillate; **critically damped** return fastest without overshoot; **overdamped** return more slowly.

> [!equation]
> - **Equation of motion (damped):** $\displaystyle m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0$
> - **Underdamped solution:** $\displaystyle x(t) = A_0 e^{-\frac{b}{2m}t}\cos(\omega t + \phi)$

> [!note] Connection
> Resistance damps electrical oscillations the same way in RLC circuits — [[Inductance]].

## Forced Oscillations
- The **natural frequency** is how a system oscillates with no driving or damping.
- Driving at the natural frequency gives **resonance**; less damping gives a taller, sharper peak.

> [!equation]
> - **Amplitude (forced, damped):** $\displaystyle A = \frac{F_o}{\sqrt{m^2(\omega^2 - \omega_o^2)^2 + b^2\omega^2}}$

> [!note] Connection
> Electrical resonance is in [[Alternating-Current Circuits]].

## See Also
- [[Eigenvalues and Eigenvectors]] (Linear Algebra)
- [[Waves]]
- [[Newton's Laws of Motion]]
- [[Inductance]]

## Sources
- [Chapter 15 Summary — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/15-summary)
- [Chapter 15 Key Equations — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/15-key-equations)
