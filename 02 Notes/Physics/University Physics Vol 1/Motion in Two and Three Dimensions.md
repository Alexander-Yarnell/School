---
aliases: [Ch. 4 Motion in Two and Three Dimensions, 2D Kinematics, Projectile Motion, Circular Motion, Relative Motion]
tags: [physics, mechanics, up-vol1]
unit: Mechanics
chapter: 4
---
# Motion in Two and Three Dimensions

> [!info] [[University Physics Vol 1]] › Unit 1 — Mechanics › Chapter 4
> ← [[Motion Along a Straight Line]] · Next: [[Newton's Laws of Motion]] →

**Motion in Two and Three Dimensions** extends [[Motion Along a Straight Line]] using [[Vectors]], covering projectiles, circular motion and motion seen from different reference frames.

## Key Equations

> [!equation]
> - **Position vector:** $\displaystyle \vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}$
> - **Velocity vector:** $\displaystyle \vec{v}(t) = \frac{d\vec{r}}{dt}$
> - **Acceleration vector:** $\displaystyle \vec{a}(t) = \frac{d\vec{v}(t)}{dt}$
> - **Time of flight:** $\displaystyle T_{\text{tof}} = \frac{2(v_0\sin\theta_0)}{g}$
> - **Trajectory:** $\displaystyle y = (\tan\theta_0)x - \left[\frac{g}{2(v_0\cos\theta_0)^2}\right]x^2$
> - **Range:** $\displaystyle R = \frac{v_0^2\sin 2\theta_0}{g}$
> - **Centripetal acceleration:** $\displaystyle a_C = \frac{v^2}{r}$
> - **Tangential acceleration:** $\displaystyle a_T = \frac{d|\vec{v}|}{dt}$
> - **Total acceleration:** $\displaystyle \vec{a} = \vec{a}_C + \vec{a}_T$
> - **Position in uniform circular motion:** $\displaystyle \vec{r}(t) = A\cos\omega t\,\hat{i} + A\sin\omega t\,\hat{j}$
> - **Relative velocity:** $\displaystyle \vec{v}_{PS} = \vec{v}_{PS'} + \vec{v}_{S'S}$
> - **Relative acceleration:** $\displaystyle \vec{a}_{PS} = \vec{a}_{PS'} + \vec{a}_{S'S}$

---

## Displacement and Velocity Vectors
- The **position vector** locates a particle relative to the origin; the **displacement vector** is the shortest path between two positions.
- Velocity is a vector tangent to the trajectory.
- Motion along one axis is **independent** of motion along a perpendicular axis.

> [!equation]
> - **Position vector:** $\displaystyle \vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}$
> - **Velocity vector:** $\displaystyle \vec{v}(t) = \frac{d\vec{r}}{dt}$

## Acceleration Vector
- In 2D and 3D, acceleration can point in any direction, not necessarily along the velocity.
- The constant-acceleration equations apply separately along each axis.

> [!equation]
> - **Acceleration vector:** $\displaystyle \vec{a}(t) = \frac{d\vec{v}(t)}{dt}$

## Projectile Motion
- A **projectile** is acted on only by gravity, which is constant near Earth's surface.
- Solve horizontal and vertical motion separately with 1D kinematics.
- The time-of-flight and range formulas apply only when the projectile lands at its launch height.

> [!equation]
> - **Time of flight:** $\displaystyle T_{\text{tof}} = \frac{2(v_0\sin\theta_0)}{g}$
> - **Trajectory:** $\displaystyle y = (\tan\theta_0)x - \left[\frac{g}{2(v_0\cos\theta_0)^2}\right]x^2$
> - **Range:** $\displaystyle R = \frac{v_0^2\sin 2\theta_0}{g}$

## Uniform and Nonuniform Circular Motion
- **Uniform circular motion** is circular motion at constant speed; its **centripetal acceleration** points to the center.
- In **nonuniform** circular motion, a **tangential acceleration** changes the speed; the total acceleration is the vector sum of the two.

> [!equation]
> - **Centripetal acceleration:** $\displaystyle a_C = \frac{v^2}{r}$
> - **Tangential acceleration:** $\displaystyle a_T = \frac{d|\vec{v}|}{dt}$
> - **Total acceleration:** $\displaystyle \vec{a} = \vec{a}_C + \vec{a}_T$
> - **Position in uniform circular motion:** $\displaystyle \vec{r}(t) = A\cos\omega t\,\hat{i} + A\sin\omega t\,\hat{j}$

> [!note] Connection
> The force that produces centripetal acceleration is covered in [[Applications of Newton's Laws]]. The angular description ($\omega$, $\alpha$) is in [[Fixed-Axis Rotation]], and the projection of circular motion onto an axis is simple harmonic motion — see [[Oscillations]].

## Relative Motion
- Position, velocity and acceleration must be stated relative to a **reference frame**.
- For frames moving at constant relative velocity, velocities add as below and acceleration is the same in both frames.

> [!equation]
> - **Relative velocity:** $\displaystyle \vec{v}_{PS} = \vec{v}_{PS'} + \vec{v}_{S'S}$
> - **Relative acceleration:** $\displaystyle \vec{a}_{PS} = \vec{a}_{PS'} + \vec{a}_{S'S}$

## See Also
- [[Linear Transformations]] (Linear Algebra)
- [[Motion Along a Straight Line]]
- [[Vectors]]
- [[Applications of Newton's Laws]]

## Sources
- [Chapter 4 Summary — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/4-summary)
- [Chapter 4 Key Equations — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/4-key-equations)
