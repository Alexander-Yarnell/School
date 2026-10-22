---
aliases: [Ch. 10 Fixed-Axis Rotation, Rotation, Rotational Kinematics, Moment of Inertia, Torque, Rotational Kinetic Energy]
tags: [physics, mechanics, up-vol1]
unit: Mechanics
chapter: 10
---
# Fixed-Axis Rotation

> [!info] [[University Physics Vol 1]] › Unit 1 — Mechanics › Chapter 10
> ← [[Linear Momentum and Collisions]] · Next: [[Angular Momentum]] →

**Fixed-Axis Rotation** builds the rotational versions of kinematics and dynamics: angle, angular velocity, angular acceleration, moment of inertia and torque.

## Key Equations

> [!equation]
> - **Angular position:** $\displaystyle \theta = \frac{s}{r}$
> - **Angular velocity:** $\displaystyle \omega = \frac{d\theta}{dt}$
> - **Tangential speed:** $\displaystyle v_t = r\omega$
> - **Angular acceleration:** $\displaystyle \alpha = \frac{d\omega}{dt} = \frac{d^2\theta}{dt^2}$
> - **Tangential acceleration:** $\displaystyle a_t = r\alpha$
> - **Angular velocity:** $\displaystyle \omega_f = \omega_0 + \alpha t$
> - **Angular displacement:** $\displaystyle \theta_f = \theta_0 + \omega_0 t + \tfrac{1}{2}\alpha t^2$
> - **Angular velocity from displacement:** $\displaystyle \omega_f^2 = \omega_0^2 + 2\alpha\,\Delta\theta$
> - **Total acceleration:** $\displaystyle \vec{a} = \vec{a}_c + \vec{a}_t$
> - **Moment of inertia:** $\displaystyle I = \sum_j m_j r_j^2$
> - **Rotational kinetic energy:** $\displaystyle K = \tfrac{1}{2}I\omega^2$
> - **Moment of inertia (continuous):** $\displaystyle I = \int r^2\,dm$
> - **Parallel-axis theorem:** $\displaystyle I_{\text{parallel-axis}} = I_{\text{CM}} + md^2$
> - **Torque:** $\displaystyle \vec{\tau} = \vec{r} \times \vec{F}$
> - **Magnitude of torque:** $\displaystyle |\vec{\tau}| = r_\perp F$
> - **Newton's second law for rotation:** $\displaystyle \sum_i \tau_i = I\alpha$
> - **Rotational work:** $\displaystyle W_{AB} = \int_{\theta_A}^{\theta_B} \left(\sum_i \tau_i\right)d\theta$
> - **Rotational power:** $\displaystyle P = \tau\omega$

---

## Rotational Variables
- **Angular position** $\theta$, **angular velocity** $\omega$ (rad/s) and **angular acceleration** $\alpha$ are the rotational analogs of $x$, $v$, $a$.
- The direction of $\omega$ follows the right-hand rule.
- A point at radius $r$ has tangential speed $r\omega$ and tangential acceleration $r\alpha$.

> [!equation]
> - **Angular position:** $\displaystyle \theta = \frac{s}{r}$
> - **Angular velocity:** $\displaystyle \omega = \frac{d\theta}{dt}$
> - **Tangential speed:** $\displaystyle v_t = r\omega$
> - **Angular acceleration:** $\displaystyle \alpha = \frac{d\omega}{dt} = \frac{d^2\theta}{dt^2}$
> - **Tangential acceleration:** $\displaystyle a_t = r\alpha$

## Rotation with Constant Angular Acceleration
- With constant $\alpha$, $\omega$ varies linearly, so the average is the mean of the start and end values.
- These equations mirror the linear ones in [[Motion Along a Straight Line]] with $x\to\theta$, $v\to\omega$, $a\to\alpha$.

> [!equation]
> - **Angular velocity:** $\displaystyle \omega_f = \omega_0 + \alpha t$
> - **Angular displacement:** $\displaystyle \theta_f = \theta_0 + \omega_0 t + \tfrac{1}{2}\alpha t^2$
> - **Angular velocity from displacement:** $\displaystyle \omega_f^2 = \omega_0^2 + 2\alpha\,\Delta\theta$

## Relating Angular and Translational Quantities
- In uniform circular motion $\omega$ is constant but points still have centripetal acceleration.
- In nonuniform circular motion there is also tangential acceleration; the two are perpendicular.

> [!equation]
> - **Total acceleration:** $\displaystyle \vec{a} = \vec{a}_c + \vec{a}_t$

> [!note] Connection
> Compare [[Motion in Two and Three Dimensions]].

## Moment of Inertia and Rotational Kinetic Energy
- The **moment of inertia** $I$ is the rotational counterpart of mass; it grows with the square of distance from the axis.
- Without non-conservative forces, total mechanical energy (translational + rotational KE + PE) is conserved.

> [!equation]
> - **Moment of inertia:** $\displaystyle I = \sum_j m_j r_j^2$
> - **Rotational kinetic energy:** $\displaystyle K = \tfrac{1}{2}I\omega^2$

> [!note] Connection
> Compare $K = \tfrac12 mv^2$ in [[Work and Kinetic Energy]].

## Calculating Moments of Inertia
- Integrate $r^2$ over the mass; mass farther from the axis means larger $I$.
- The **parallel-axis theorem** shifts the axis; a compound object's $I$ is the sum of its parts.

> [!equation]
> - **Moment of inertia (continuous):** $\displaystyle I = \int r^2\,dm$
> - **Parallel-axis theorem:** $\displaystyle I_{\text{parallel-axis}} = I_{\text{CM}} + md^2$

## Torque
- Torque magnitude is $r_\perp F$, where $r_\perp$ is the lever arm; the sign follows the right-hand rule.
- Net torque is the sum of individual torques about an axis.

> [!equation]
> - **Torque:** $\displaystyle \vec{\tau} = \vec{r} \times \vec{F}$
> - **Magnitude of torque:** $\displaystyle |\vec{\tau}| = r_\perp F$

> [!note] Connection
> Torque uses the cross product from [[Vectors]]. Torque on a current loop, $\vec\tau = \vec\mu\times\vec B$, is in [[Magnetic Forces and Fields]].

## Newton's Second Law for Rotation
- For a fixed axis, net torque equals moment of inertia times angular acceleration; torque and $\alpha$ point the same way.

> [!equation]
> - **Newton's second law for rotation:** $\displaystyle \sum_i \tau_i = I\alpha$

> [!note] Connection
> Rotational analog of $\vec F = m\vec a$ — [[Newton's Laws of Motion]].

## Work and Power for Rotational Motion
- Incremental work is $dW = \tau\,d\theta$; the work-energy theorem holds for rotation.
- Power delivered to a rotating body is torque times angular velocity.

> [!equation]
> - **Rotational work:** $\displaystyle W_{AB} = \int_{\theta_A}^{\theta_B} \left(\sum_i \tau_i\right)d\theta$
> - **Rotational power:** $\displaystyle P = \tau\omega$

## See Also
- [[Linear Transformations]] (Linear Algebra)
- [[Angular Momentum]]
- [[Static Equilibrium and Elasticity]]
- [[Work and Kinetic Energy]]

## Sources
- [Chapter 10 Summary — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/10-summary)
- [Chapter 10 Key Equations — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/10-key-equations)
