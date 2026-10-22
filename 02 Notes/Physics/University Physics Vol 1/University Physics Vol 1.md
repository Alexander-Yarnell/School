---
aliases: [UP Vol 1, University Physics Volume 1]
tags: [physics, openstax, index]
---
# University Physics Volume 1

*University Physics* is a free, three-volume, calculus-based physics series by Samuel J. Ling, William Moebs and Jeff Sanny, published by OpenStax (Rice University). **Volume 1** has two units and 17 chapters: fourteen on **Mechanics** and three on **Waves and Acoustics**.

> [!tip] How to read these notes
> The important equations to know and use are in pink **equation** boxes. Every chapter page lists all of its key equations at the top, then repeats each one in the notes where it comes up.
> The boxes turn pink when the `pink-equations` CSS snippet is on (Settings → Appearance → CSS snippets).

---

## Key Equations

### Mechanics

> [!equation] [[Units and Measurement]]
> - **Percent uncertainty:** $\displaystyle \text{Percent uncertainty} = \frac{\delta A}{A} \times 100\%$

> [!equation] [[Vectors]]
> - **Component form (3D):** $\displaystyle \vec{A} = A_x \hat{i} + A_y \hat{j} + A_z \hat{k}$
> - **Magnitude:** $\displaystyle A = \sqrt{A_x^2 + A_y^2 + A_z^2}$
> - **Direction angle in a plane:** $\displaystyle \theta_A = \tan^{-1}\left(\frac{A_y}{A_x}\right)$
> - **Scalar (dot) product:** $\displaystyle \vec{A} \cdot \vec{B} = AB\cos\varphi = A_x B_x + A_y B_y + A_z B_z$
> - **Magnitude of the vector (cross) product:** $\displaystyle |\vec{A} \times \vec{B}| = AB\sin\varphi$

> [!equation] [[Motion Along a Straight Line]]
> - **Average velocity:** $\displaystyle \bar{v} = \frac{\Delta x}{\Delta t} = \frac{x_2 - x_1}{t_2 - t_1}$
> - **Instantaneous velocity:** $\displaystyle v(t) = \frac{dx(t)}{dt}$
> - **Instantaneous acceleration:** $\displaystyle a(t) = \frac{dv(t)}{dt}$
> - **Velocity from acceleration:** $\displaystyle v = v_0 + at$
> - **Position from velocity and acceleration:** $\displaystyle x = x_0 + v_0 t + \frac{1}{2}at^2$
> - **Velocity from distance:** $\displaystyle v^2 = v_0^2 + 2a(x - x_0)$

> [!equation] [[Motion in Two and Three Dimensions]]
> - **Velocity vector:** $\displaystyle \vec{v}(t) = \frac{d\vec{r}}{dt}$
> - **Acceleration vector:** $\displaystyle \vec{a}(t) = \frac{d\vec{v}(t)}{dt}$
> - **Range:** $\displaystyle R = \frac{v_0^2\sin 2\theta_0}{g}$
> - **Centripetal acceleration:** $\displaystyle a_C = \frac{v^2}{r}$
> - **Relative velocity:** $\displaystyle \vec{v}_{PS} = \vec{v}_{PS'} + \vec{v}_{S'S}$

> [!equation] [[Newton's Laws of Motion]]
> - **Newton's second law:** $\displaystyle \vec{F}_{\text{net}} = \sum \vec{F} = m\vec{a}$
> - **Weight:** $\displaystyle w = mg$
> - **Newton's third law:** $\displaystyle \vec{F}_{AB} = -\vec{F}_{BA}$
> - **Hooke's law (spring force):** $\displaystyle \vec{F} = -k\vec{x}$

> [!equation] [[Applications of Newton's Laws]]
> - **Static friction:** $\displaystyle f_s \le \mu_s N$
> - **Kinetic friction:** $\displaystyle f_k = \mu_k N$
> - **Centripetal force:** $\displaystyle F_c = m\frac{v^2}{r} = mr\omega^2$
> - **Drag force:** $\displaystyle F_D = \frac{1}{2}C\rho A v^2$

> [!equation] [[Work and Kinetic Energy]]
> - **Work (infinitesimal):** $\displaystyle dW = \vec{F} \cdot d\vec{r} = |\vec{F}|\,|d\vec{r}|\cos\theta$
> - **Work along a path:** $\displaystyle W_{AB} = \int_{\text{path } AB} \vec{F} \cdot d\vec{r}$
> - **Kinetic energy:** $\displaystyle K = \tfrac{1}{2}mv^2 = \frac{p^2}{2m}$
> - **Work-energy theorem:** $\displaystyle W_{\text{net}} = K_B - K_A$
> - **Power:** $\displaystyle P = \frac{dW}{dt}$

> [!equation] [[Potential Energy and Conservation of Energy]]
> - **Potential energy difference:** $\displaystyle \Delta U_{AB} = U_B - U_A = -W_{AB}$
> - **Gravitational PE near Earth:** $\displaystyle U(y) = mgy + \text{const.}$
> - **Spring PE:** $\displaystyle U(x) = \tfrac{1}{2}kx^2 + \text{const.}$
> - **Force from potential energy:** $\displaystyle F_l = -\frac{dU}{dl}$
> - **Conservation of energy:** $\displaystyle 0 = W_{nc,AB} = \Delta(K+U)_{AB} = \Delta E_{AB}$

> [!equation] [[Linear Momentum and Collisions]]
> - **Momentum:** $\displaystyle \vec{p} = m\vec{v}$
> - **Impulse:** $\displaystyle \vec{J} = \int_{t_i}^{t_f} \vec{F}(t)\,dt = \vec{F}_{\text{ave}}\,\Delta t$
> - **Impulse-momentum theorem:** $\displaystyle \vec{J} = \Delta\vec{p}$
> - **Conservation of momentum:** $\displaystyle \vec{p}_1 + \vec{p}_2 = \text{constant}$
> - **Center of mass (particles):** $\displaystyle \vec{r}_{\text{CM}} = \frac{1}{M}\sum_{j=1}^{N} m_j\vec{r}_j$
> - **Rocket equation:** $\displaystyle \Delta v = u\ln\left(\frac{m_i}{m}\right)$

> [!equation] [[Fixed-Axis Rotation]]
> - **Angular velocity:** $\displaystyle \omega = \frac{d\theta}{dt}$
> - **Tangential speed:** $\displaystyle v_t = r\omega$
> - **Angular velocity:** $\displaystyle \omega_f = \omega_0 + \alpha t$
> - **Angular displacement:** $\displaystyle \theta_f = \theta_0 + \omega_0 t + \tfrac{1}{2}\alpha t^2$
> - **Moment of inertia:** $\displaystyle I = \sum_j m_j r_j^2$
> - **Rotational kinetic energy:** $\displaystyle K = \tfrac{1}{2}I\omega^2$
> - **Parallel-axis theorem:** $\displaystyle I_{\text{parallel-axis}} = I_{\text{CM}} + md^2$
> - **Torque:** $\displaystyle \vec{\tau} = \vec{r} \times \vec{F}$
> - **Newton's second law for rotation:** $\displaystyle \sum_i \tau_i = I\alpha$
> - **Rotational power:** $\displaystyle P = \tau\omega$

> [!equation] [[Angular Momentum]]
> - **Rolling without slipping:** $\displaystyle v_{\text{CM}} = R\omega,\quad a_{\text{CM}} = R\alpha$
> - **Angular momentum (particle):** $\displaystyle \vec{l} = \vec{r} \times \vec{p}$
> - **Torque and angular momentum:** $\displaystyle \frac{d\vec{L}}{dt} = \sum \vec{\tau}$
> - **Angular momentum (rigid body):** $\displaystyle L = I\omega$
> - **Conservation of angular momentum:** $\displaystyle \frac{d\vec{L}}{dt} = 0 \;\Rightarrow\; \vec{L} = \text{constant}$

> [!equation] [[Static Equilibrium and Elasticity]]
> - **First equilibrium condition:** $\displaystyle \sum_k \vec{F}_k = \vec{0}$
> - **Second equilibrium condition:** $\displaystyle \sum_k \vec{\tau}_k = \vec{0}$
> - **Stress and strain:** $\displaystyle \text{stress} = (\text{elastic modulus}) \times \text{strain}$
> - **Young's modulus:** $\displaystyle Y = \frac{F_\perp}{A}\,\frac{L_0}{\Delta L}$

> [!equation] [[Gravitation]]
> - **Newton's law of gravitation:** $\displaystyle \vec{F}_{12} = G\frac{m_1 m_2}{r^2}\hat{r}_{12}$
> - **Gravity at Earth's surface:** $\displaystyle g = G\frac{M_E}{r^2}$
> - **Gravitational PE:** $\displaystyle U = -\frac{GM_E m}{r}$
> - **Escape velocity:** $\displaystyle v_{\text{esc}} = \sqrt{\frac{2GM}{R}}$
> - **Orbital speed:** $\displaystyle v_{\text{orbit}} = \sqrt{\frac{GM_E}{r}}$
> - **Kepler's third law:** $\displaystyle T^2 = \frac{4\pi^2}{GM}a^3$

> [!equation] [[Fluid Mechanics]]
> - **Density:** $\displaystyle \rho = \frac{m}{V}$
> - **Pressure:** $\displaystyle p = \frac{F}{A}$
> - **Pressure at depth:** $\displaystyle p = p_0 + \rho g h$
> - **Pascal's principle:** $\displaystyle \frac{F_1}{A_1} = \frac{F_2}{A_2}$
> - **Continuity equation:** $\displaystyle A_1 v_1 = A_2 v_2$
> - **Bernoulli's equation:** $\displaystyle p + \tfrac{1}{2}\rho v^2 + \rho g y = \text{constant}$
> - **Poiseuille's law:** $\displaystyle Q = \frac{(p_2 - p_1)\pi r^4}{8\eta l}$

### Waves and Acoustics

> [!equation] [[Oscillations]]
> - **Frequency and period:** $\displaystyle f = \frac{1}{T}$
> - **Position in SHM:** $\displaystyle x(t) = A\cos(\omega t + \phi)$
> - **Angular frequency (mass-spring):** $\displaystyle \omega = \sqrt{\frac{k}{m}}$
> - **Period (mass-spring):** $\displaystyle T = 2\pi\sqrt{\frac{m}{k}}$
> - **Total energy (mass-spring):** $\displaystyle E_{\text{Total}} = \tfrac{1}{2}kx^2 + \tfrac{1}{2}mv^2 = \tfrac{1}{2}kA^2$
> - **Period (simple pendulum):** $\displaystyle T = 2\pi\sqrt{\frac{L}{g}}$

> [!equation] [[Waves]]
> - **Wave speed:** $\displaystyle v = \frac{\lambda}{T} = \lambda f$
> - **Wave function:** $\displaystyle y(x,t) = A\sin(kx \mp \omega t + \phi)$
> - **Speed on a string:** $\displaystyle v = \sqrt{\frac{F_T}{\mu}}$
> - **Intensity:** $\displaystyle I = \frac{P}{A}$
> - **Wavelengths (both ends fixed):** $\displaystyle \lambda_n = \frac{2}{n}L$
> - **Frequencies (both ends fixed):** $\displaystyle f_n = n\frac{v}{2L} = nf_1$

> [!equation] [[Sound]]
> - **Wave speed:** $\displaystyle v = f\lambda$
> - **Speed in an ideal gas:** $\displaystyle v = \sqrt{\frac{\gamma RT}{M}}$
> - **Sound intensity level:** $\displaystyle \beta\,(\text{dB}) = 10\log_{10}\left(\frac{I}{I_0}\right)$
> - **Tube closed at one end:** $\displaystyle f_n = n\frac{v}{4L},\quad n = 1, 3, 5, \ldots$
> - **Tube open at both ends:** $\displaystyle f_n = n\frac{v}{2L},\quad n = 1, 2, 3, \ldots$
> - **Beat frequency:** $\displaystyle f_{\text{beat}} = |f_2 - f_1|$
> - **Doppler shift:** $\displaystyle f_o = f_s\left(\frac{v \pm v_o}{v \mp v_s}\right)$

---

## Unit 1 — Mechanics

How things move and why: measurement and vectors, kinematics, Newton's laws, energy, momentum, rotation, gravity and fluids.

1. [[Units and Measurement]] — scope of physics; SI units; unit conversion; dimensional analysis; estimates; significant figures; problem solving.
2. [[Vectors]] — scalars and vectors; components; vector algebra; dot and cross products.
3. [[Motion Along a Straight Line]] — displacement; velocity and speed; acceleration; constant-acceleration equations; free fall; calculus of motion.
4. [[Motion in Two and Three Dimensions]] — position, velocity and acceleration vectors; projectile motion; circular motion; relative motion.
5. [[Newton's Laws of Motion]] — forces; the three laws; mass and weight; normal force, tension, springs; free-body diagrams.
6. [[Applications of Newton's Laws]] — problem solving with Newton's laws; friction; centripetal force; drag and terminal speed.
7. [[Work and Kinetic Energy]] — work; kinetic energy; the work-energy theorem; power.
8. [[Potential Energy and Conservation of Energy]] — potential energy; conservative vs non-conservative forces; energy conservation; energy diagrams and stability; energy sources.
9. [[Linear Momentum and Collisions]] — momentum; impulse; conservation of momentum; elastic and inelastic collisions; center of mass; rockets.
10. [[Fixed-Axis Rotation]] — angular variables; constant angular acceleration; moment of inertia; torque; Newton's second law for rotation; rotational work and power.
11. [[Angular Momentum]] — rolling motion; angular momentum; its conservation; gyroscope precession.
12. [[Static Equilibrium and Elasticity]] — conditions for equilibrium; worked examples; stress, strain and elastic moduli; elasticity and plasticity.
13. [[Gravitation]] — universal gravitation; gravity near Earth; gravitational energy; orbits; Kepler's laws; tides; Einstein's theory of gravity.
14. [[Fluid Mechanics]] — density and pressure; measuring pressure; Pascal's principle; buoyancy; fluid flow; Bernoulli's equation; viscosity and turbulence.

## Unit 2 — Waves and Acoustics

Repeating motion and the disturbances it sends through a medium: oscillations, waves and sound.

15. [[Oscillations]] — simple harmonic motion; energy in SHM; link to circular motion; pendulums; damping; forced oscillations and resonance.
16. [[Waves]] — traveling waves; wave functions; wave speed on a string; energy and power; interference; standing waves and resonance.
17. [[Sound]] — sound waves; speed of sound; intensity and decibels; standing sound waves; musical sound; beats; Doppler effect; shock waves.

## The Other Volumes
- [[University Physics Vol 2]] — thermodynamics (Ch. 1–4) and electricity and magnetism (Ch. 5–16).
- [[University Physics Vol 3]] — optics (Ch. 1–4) and modern physics (Ch. 5–11).

## Sources
- [University Physics Volume 1 — OpenStax](https://openstax.org/details/books/university-physics-volume-1)
- [Volume 3 preface: coverage and scope (chapter list for all three volumes)](https://openstax.org/books/university-physics-volume-3/pages/preface)
- Each chapter page lists the OpenStax summary and key-equations pages it was built from.
