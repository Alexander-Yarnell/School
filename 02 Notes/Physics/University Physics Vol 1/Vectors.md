---
aliases: [Ch. 2 Vectors, Vector, Dot Product, Cross Product, Scalar Product, Vector Product]
tags: [physics, mechanics, up-vol1]
unit: Mechanics
chapter: 2
---
# Vectors

> [!info] [[University Physics Vol 1]] › Unit 1 — Mechanics › Chapter 2
> ← [[Units and Measurement]] · Next: [[Motion Along a Straight Line]] →

**Vectors** are quantities with both magnitude and direction. This chapter covers how to add them, break them into components, and multiply them — tools used in every later chapter.

## Key Equations

> [!equation]
> - **Multiplication by a scalar:** $\displaystyle \vec{B} = \alpha \vec{A}$
> - **Magnitude after scalar multiplication:** $\displaystyle B = |\alpha| A$
> - **Commutative law:** $\displaystyle \vec{A} + \vec{B} = \vec{B} + \vec{A}$
> - **Associative law:** $\displaystyle (\vec{A} + \vec{B}) + \vec{C} = \vec{A} + (\vec{B} + \vec{C})$
> - **Distributive law:** $\displaystyle \alpha_1 \vec{A} + \alpha_2 \vec{A} = (\alpha_1 + \alpha_2)\vec{A}$
> - **Component form (3D):** $\displaystyle \vec{A} = A_x \hat{i} + A_y \hat{j} + A_z \hat{k}$
> - **Magnitude:** $\displaystyle A = \sqrt{A_x^2 + A_y^2 + A_z^2}$
> - **Direction angle in a plane:** $\displaystyle \theta_A = \tan^{-1}\left(\frac{A_y}{A_x}\right)$
> - **Components from magnitude and angle:** $\displaystyle A_x = A\cos\theta_A,\quad A_y = A\sin\theta_A$
> - **Polar coordinates:** $\displaystyle x = r\cos\varphi,\quad y = r\sin\varphi$
> - **General unit vector:** $\displaystyle \hat{V} = \frac{\vec{V}}{V}$
> - **Resultant of N vectors (x-component):** $\displaystyle F_{Rx} = \sum_{k=1}^{N} F_{kx}$
> - **Scalar (dot) product:** $\displaystyle \vec{A} \cdot \vec{B} = AB\cos\varphi = A_x B_x + A_y B_y + A_z B_z$
> - **Angle between two vectors:** $\displaystyle \cos\varphi = \frac{\vec{A} \cdot \vec{B}}{AB}$
> - **Magnitude of the vector (cross) product:** $\displaystyle |\vec{A} \times \vec{B}| = AB\sin\varphi$
> - **Anticommutative property:** $\displaystyle \vec{A} \times \vec{B} = -\vec{B} \times \vec{A}$
> - **Cross product in components:** $\displaystyle \vec{A} \times \vec{B} = (A_y B_z - A_z B_y)\hat{i} + (A_z B_x - A_x B_z)\hat{j} + (A_x B_y - A_y B_x)\hat{k}$

---

## Scalars and Vectors
- Vectors have magnitude and direction (e.g. displacement, velocity) and are drawn as arrows.
- Two vectors are equal only if both magnitude and direction match. **Parallel** vectors share direction, **antiparallel** differ by 180°, **orthogonal** by 90°.
- Multiplying by a positive scalar changes only the magnitude; a negative scalar also reverses direction.
- Vectors add to give a **resultant**. Addition is commutative and associative; geometrically use the parallelogram rule or tail-to-head method.

> [!equation]
> - **Multiplication by a scalar:** $\displaystyle \vec{B} = \alpha \vec{A}$
> - **Magnitude after scalar multiplication:** $\displaystyle B = |\alpha| A$
> - **Commutative law:** $\displaystyle \vec{A} + \vec{B} = \vec{B} + \vec{A}$
> - **Associative law:** $\displaystyle (\vec{A} + \vec{B}) + \vec{C} = \vec{A} + (\vec{B} + \vec{C})$
> - **Distributive law:** $\displaystyle \alpha_1 \vec{A} + \alpha_2 \vec{A} = (\alpha_1 + \alpha_2)\vec{A}$

## Coordinate Systems and Components
- A vector is the sum of its components — two in a plane, three in space.
- In a plane, the direction is the counterclockwise angle from the +x-axis; $A_x = A\cos\theta_A$, $A_y = A\sin\theta_A$.
- The Cartesian system uses unit vectors $\hat{i}, \hat{j}, \hat{k}$; the polar system uses radial and perpendicular unit vectors.

> [!equation]
> - **Component form (3D):** $\displaystyle \vec{A} = A_x \hat{i} + A_y \hat{j} + A_z \hat{k}$
> - **Magnitude:** $\displaystyle A = \sqrt{A_x^2 + A_y^2 + A_z^2}$
> - **Direction angle in a plane:** $\displaystyle \theta_A = \tan^{-1}\left(\frac{A_y}{A_x}\right)$
> - **Components from magnitude and angle:** $\displaystyle A_x = A\cos\theta_A,\quad A_y = A\sin\theta_A$
> - **Polar coordinates:** $\displaystyle x = r\cos\varphi,\quad y = r\sin\varphi$
> - **General unit vector:** $\displaystyle \hat{V} = \frac{\vec{V}}{V}$

## Algebra of Vectors
- Analytical (component) methods give exact resultants without drawing; graphical methods are approximate.
- Add vectors by adding their components along each axis.
- These methods are used throughout mechanics and electricity and magnetism.

> [!equation]
> - **Resultant of N vectors (x-component):** $\displaystyle F_{Rx} = \sum_{k=1}^{N} F_{kx}$

## Products of Vectors
- The **scalar (dot) product** gives a number; the **vector (cross) product** gives a vector.
- Both are distributive. The dot product is commutative; the cross product is **anticommutative** (swapping order flips the sign).
- Dot product: zero for orthogonal vectors, negative for antiparallel ones.
- Cross product: perpendicular to both vectors (right-hand rule); zero for parallel vectors, largest for orthogonal ones.

> [!equation]
> - **Scalar (dot) product:** $\displaystyle \vec{A} \cdot \vec{B} = AB\cos\varphi = A_x B_x + A_y B_y + A_z B_z$
> - **Angle between two vectors:** $\displaystyle \cos\varphi = \frac{\vec{A} \cdot \vec{B}}{AB}$
> - **Magnitude of the vector (cross) product:** $\displaystyle |\vec{A} \times \vec{B}| = AB\sin\varphi$
> - **Anticommutative property:** $\displaystyle \vec{A} \times \vec{B} = -\vec{B} \times \vec{A}$
> - **Cross product in components:** $\displaystyle \vec{A} \times \vec{B} = (A_y B_z - A_z B_y)\hat{i} + (A_z B_x - A_x B_z)\hat{j} + (A_x B_y - A_y B_x)\hat{k}$

> [!note] Connection
> The dot product is used to define **work** — see [[Work and Kinetic Energy]]. The cross product is used for **torque** ([[Fixed-Axis Rotation]]), **angular momentum** ([[Angular Momentum]]) and **magnetic force** ([[Magnetic Forces and Fields]]).

## See Also
- [[Vectors in Rn]] (Linear Algebra)
- [[Determinants]] (Linear Algebra)
- [[Motion in Two and Three Dimensions]]
- [[Work and Kinetic Energy]]
- [[Fixed-Axis Rotation]]

## Sources
- [Chapter 2 Summary — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/2-summary)
- [Chapter 2 Key Equations — OpenStax University Physics Volume 1](https://openstax.org/books/university-physics-volume-1/pages/2-key-equations)
