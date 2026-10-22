---
aliases: [Ch. 7 Quantum Mechanics, Wave Function, Schrodinger Equation, Schrödinger Equation, Uncertainty Principle, Particle in a Box, Quantum Tunneling]
tags: [physics, modern-physics, up-vol3]
unit: Modern Physics
chapter: 7
---
# Quantum Mechanics

> [!info] [[University Physics Vol 3]] › Unit 2 — Modern Physics › Chapter 7
> ← [[Photons and Matter Waves]] · Next: [[Atomic Structure]] →

**Quantum Mechanics** replaces trajectories with wave functions. The Schrödinger equation predicts them, and solving it gives quantized energies, zero-point motion and tunneling.

## Key Equations

> [!equation]
> - **Normalization:** $\displaystyle \int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx = 1$
> - **Expectation value of position:** $\displaystyle \langle x\rangle = \int_{-\infty}^{\infty}\Psi^*(x,t)\,x\,\Psi(x,t)\,dx$
> - **Position–momentum uncertainty:** $\displaystyle \Delta x\,\Delta p \ge \frac{\hbar}{2}$
> - **Energy–time uncertainty:** $\displaystyle \Delta E\,\Delta t \ge \frac{\hbar}{2}$
> - **Time-dependent Schrödinger equation:** $\displaystyle -\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2} + U\Psi = i\hbar\frac{\partial\Psi}{\partial t}$
> - **Time-independent Schrödinger equation:** $\displaystyle -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + U(x)\psi = E\psi$
> - **Allowed energies:** $\displaystyle E_n = n^2\frac{\pi^2\hbar^2}{2mL^2},\quad n = 1, 2, 3, \ldots$
> - **Stationary states:** $\displaystyle \psi_n(x) = \sqrt{\frac{2}{L}}\sin\frac{n\pi x}{L}$
> - **Potential energy:** $\displaystyle U(x) = \tfrac{1}{2}m\omega^2x^2$
> - **Energy levels:** $\displaystyle E_n = \left(n + \tfrac{1}{2}\right)\hbar\omega,\quad n = 0, 1, 2, \ldots$
> - **Transmission coefficient (approx.):** $\displaystyle T(L,E) = 16\frac{E}{U_0}\left(1 - \frac{E}{U_0}\right)e^{-2\beta L}$
> - **Decay parameter:** $\displaystyle \beta^2 = \frac{2m}{\hbar^2}(U_0 - E)$

---

## Wave Functions
- A quantum state is a **wave function** $\Psi$; by Born's interpretation, $|\Psi|^2$ is the probability density.
- Wave functions must be **normalized**; an **expectation value** is the average of a quantity computed from $\Psi$.

> [!equation]
> - **Normalization:** $\displaystyle \int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx = 1$
> - **Expectation value of position:** $\displaystyle \langle x\rangle = \int_{-\infty}^{\infty}\Psi^*(x,t)\,x\,\Psi(x,t)\,dx$

## The Heisenberg Uncertainty Principle
- Position and momentum can't both be known to arbitrary precision — a property of matter waves, not of the equipment.
- A short-lived state can't have a definite energy.

> [!equation]
> - **Position–momentum uncertainty:** $\displaystyle \Delta x\,\Delta p \ge \frac{\hbar}{2}$
> - **Energy–time uncertainty:** $\displaystyle \Delta E\,\Delta t \ge \frac{\hbar}{2}$

> [!note] Connection
> Introduced in [[Photons and Matter Waves]].

## The Schrödinger Equation
- The fundamental equation of wave quantum mechanics, used to predict wave functions.
- For a time-independent potential, the solution is $\psi(x)$ times a time factor $e^{-i\omega t}$.

> [!equation]
> - **Time-dependent Schrödinger equation:** $\displaystyle -\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2} + U\Psi = i\hbar\frac{\partial\Psi}{\partial t}$
> - **Time-independent Schrödinger equation:** $\displaystyle -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + U(x)\psi = E\psi$

## The Quantum Particle in a Box
- Requiring $\psi$ to vanish at the walls gives quantized energies indexed by $n$.
- At high $n$ the quantum picture matches the classical one (**correspondence principle**).

> [!equation]
> - **Allowed energies:** $\displaystyle E_n = n^2\frac{\pi^2\hbar^2}{2mL^2},\quad n = 1, 2, 3, \ldots$
> - **Stationary states:** $\displaystyle \psi_n(x) = \sqrt{\frac{2}{L}}\sin\frac{n\pi x}{L}$

> [!note] Connection
> The same result gives electron energies in a metal — [[Condensed Matter Physics]].

## The Quantum Harmonic Oscillator
- Models systems like molecular vibrations; energies are discrete and evenly spaced.
- The ground-state energy is above zero, so the oscillator is never at rest.
- There is a nonzero chance of being beyond the classical turning points.

> [!equation]
> - **Potential energy:** $\displaystyle U(x) = \tfrac{1}{2}m\omega^2x^2$
> - **Energy levels:** $\displaystyle E_n = \left(n + \tfrac{1}{2}\right)\hbar\omega,\quad n = 0, 1, 2, \ldots$

> [!note] Connection
> Classical simple harmonic motion is in [[Oscillations]].

## Quantum Tunneling
- A particle can cross a barrier higher than its energy — no classical analog.
- Probability depends on energy relative to barrier height and, exponentially, on barrier width.
- Explains radioactive decay; used in the **scanning tunneling microscope** and electronic devices.

> [!equation]
> - **Transmission coefficient (approx.):** $\displaystyle T(L,E) = 16\frac{E}{U_0}\left(1 - \frac{E}{U_0}\right)e^{-2\beta L}$
> - **Decay parameter:** $\displaystyle \beta^2 = \frac{2m}{\hbar^2}(U_0 - E)$

> [!note] Connection
> Radioactive decay is in [[Nuclear Physics]].

## See Also
- [[Eigenvalues and Eigenvectors]] (Linear Algebra)
- [[Vector Spaces]] (Linear Algebra)
- [[Photons and Matter Waves]]
- [[Atomic Structure]]
- [[Condensed Matter Physics]]

## Sources
- [Chapter 7 Summary — OpenStax University Physics Volume 3](https://openstax.org/books/university-physics-volume-3/pages/7-summary)
- [Chapter 7 Key Equations — OpenStax University Physics Volume 3](https://openstax.org/books/university-physics-volume-3/pages/7-key-equations)
