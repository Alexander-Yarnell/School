---
aliases: [R^n, Rn, Dot Product (Linear Algebra), Span, Linear Independence, Basis, Orthogonality, Gram-Schmidt, Least Squares]
tags: [mathematics, linear-algebra]
book-chapter: 4
---
# Vectors in Rn

> [!info] [[Linear Algebra]] › Kuttler Ch. 4: Rⁿ
> ← [[Determinants]] · Next: [[Linear Transformations]] →

**Vectors in $\mathbb{R}^n$** extends the arrows from physics to any number of components, then builds the key ideas of linear algebra on them: span, linear independence, basis and orthogonality.

## Key Equations

> [!equation]
> - **Length:** $\displaystyle \|\vec{u}\| = \sqrt{u_1^2 + \cdots + u_n^2}$
> - **Unit vector:** $\displaystyle \hat{u} = \frac{1}{\|\vec{v}\|}\vec{v}$
> - **Dot product:** $\displaystyle \vec{u}\cdot\vec{v} = \sum_{k=1}^{n} u_k v_k = \|\vec{u}\|\,\|\vec{v}\|\cos\theta$
> - **Cauchy–Schwarz:** $\displaystyle |\vec{u}\cdot\vec{v}| \le \|\vec{u}\|\,\|\vec{v}\|$
> - **Triangle inequality:** $\displaystyle \|\vec{u} + \vec{v}\| \le \|\vec{u}\| + \|\vec{v}\|$
> - **Projection:** $\displaystyle \operatorname{proj}_{\vec{u}}(\vec{v}) = \frac{\vec{v}\cdot\vec{u}}{\|\vec{u}\|^2}\,\vec{u}$
> - **Cross product as a determinant:** $\displaystyle \vec{u}\times\vec{v} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}$
> - **Box product (volume):** $\displaystyle V = |(\vec{u}\times\vec{v})\cdot\vec{w}|$
> - **Linear independence:** $\displaystyle \sum_{i=1}^{k} a_i\vec{u}_i = \vec{0} \;\Rightarrow\; a_1 = \cdots = a_k = 0$
> - **Fourier expansion:** $\displaystyle \vec{x} = \sum_{j=1}^{m}\frac{\vec{x}\cdot\vec{u}_j}{\|\vec{u}_j\|^2}\,\vec{u}_j$
> - **Orthogonal matrix:** $\displaystyle U^T U = UU^T = I$
> - **Gram–Schmidt step:** $\displaystyle \vec{v}_k = \vec{u}_k - \sum_{j=1}^{k-1}\frac{\vec{u}_k\cdot\vec{v}_j}{\|\vec{v}_j\|^2}\vec{v}_j$
> - **Least squares (normal equations):** $\displaystyle A^T A\vec{x} = A^T\vec{y}$
> - **Work as a dot product:** $\displaystyle W = \vec{F}\cdot(\vec{q} - \vec{p}) = \|\vec{F}\|\,\|\vec{q} - \vec{p}\|\cos\theta$

---

## Length of a Vector
- Length (norm) is the square root of the sum of squared components; distance between points is the length of the vector between them.
- A **unit vector** has length 1; dividing by the length **normalizes** a vector.

> [!equation]
> - **Length:** $\displaystyle \|\vec{u}\| = \sqrt{u_1^2 + \cdots + u_n^2}$
> - **Unit vector:** $\displaystyle \hat{u} = \frac{1}{\|\vec{v}\|}\vec{v}$

> [!note] Connection
> In 2D and 3D this is the magnitude formula from [[Vectors]].

## The Dot Product
- The dot (scalar, inner) product gives a number; $\vec{u}\cdot\vec{u} = \|\vec{u}\|^2$.
- Nonzero vectors are **orthogonal** exactly when their dot product is 0.
- **Cauchy–Schwarz** and the **triangle inequality** bound dot products and lengths.
- The **projection** of $\vec{v}$ onto $\vec{u}$ is the part of $\vec{v}$ along $\vec{u}$.

> [!equation]
> - **Dot product:** $\displaystyle \vec{u}\cdot\vec{v} = \sum_{k=1}^{n} u_k v_k = \|\vec{u}\|\,\|\vec{v}\|\cos\theta$
> - **Cauchy–Schwarz:** $\displaystyle |\vec{u}\cdot\vec{v}| \le \|\vec{u}\|\,\|\vec{v}\|$
> - **Triangle inequality:** $\displaystyle \|\vec{u} + \vec{v}\| \le \|\vec{u}\| + \|\vec{v}\|$
> - **Projection:** $\displaystyle \operatorname{proj}_{\vec{u}}(\vec{v}) = \frac{\vec{v}\cdot\vec{u}}{\|\vec{u}\|^2}\,\vec{u}$

## The Cross Product
- Defined only in $\mathbb{R}^3$; the result is perpendicular to both vectors (right-hand rule) with length $\|\vec{u}\|\|\vec{v}\|\sin\theta$.
- $\|\vec{u}\times\vec{v}\|$ is the area of the parallelogram the vectors span.
- The **box (triple) product** gives the volume of a parallelepiped and equals a 3×3 determinant.

> [!equation]
> - **Cross product as a determinant:** $\displaystyle \vec{u}\times\vec{v} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}$
> - **Box product (volume):** $\displaystyle V = |(\vec{u}\times\vec{v})\cdot\vec{w}|$

> [!note] Connection
> The cross product gives torque $\vec\tau = \vec r\times\vec F$ ([[Fixed-Axis Rotation]]), angular momentum $\vec l = \vec r\times\vec p$ ([[Angular Momentum]]) and magnetic force $\vec F = q\vec v\times\vec B$ ([[Magnetic Forces and Fields]]). Determinants are in [[Determinants]].

## Span, Linear Independence and Basis
- The **span** of a set is all its linear combinations.
- Vectors are **linearly independent** if the only combination giving $\vec 0$ uses all-zero coefficients — equivalently $A\vec{x} = \vec{0}$ has only the trivial solution.
- A **subspace** contains $\vec 0$ and is closed under addition and scalar multiplication.
- A **basis** is an independent spanning set; every basis of a subspace has the same size, its **dimension**. $\dim(\mathbb{R}^n) = n$.
- More than $n$ vectors in $\mathbb{R}^n$ are always dependent.

> [!equation]
> - **Linear independence:** $\displaystyle \sum_{i=1}^{k} a_i\vec{u}_i = \vec{0} \;\Rightarrow\; a_1 = \cdots = a_k = 0$

> [!note] Connection
> Writing a vector as $A_x\hat i + A_y\hat j + A_z\hat k$ in [[Vectors]] is expressing it in the standard basis.

## Orthogonality
- An **orthonormal** set has unit vectors that are mutually perpendicular; it is automatically independent.
- Coordinates in an orthogonal basis are found with dot products (**Fourier coefficients**).
- An **orthogonal matrix** has orthonormal columns: $U^T = U^{-1}$ and $\det U = \pm 1$.
- **Gram–Schmidt** turns any independent set into an orthogonal one with the same span.
- **Least squares:** when $A\vec{x} = \vec{y}$ has no solution, the closest fit solves the normal equations.

> [!equation]
> - **Fourier expansion:** $\displaystyle \vec{x} = \sum_{j=1}^{m}\frac{\vec{x}\cdot\vec{u}_j}{\|\vec{u}_j\|^2}\,\vec{u}_j$
> - **Orthogonal matrix:** $\displaystyle U^T U = UU^T = I$
> - **Gram–Schmidt step:** $\displaystyle \vec{v}_k = \vec{u}_k - \sum_{j=1}^{k-1}\frac{\vec{u}_k\cdot\vec{v}_j}{\|\vec{v}_j\|^2}\vec{v}_j$
> - **Least squares (normal equations):** $\displaystyle A^T A\vec{x} = A^T\vec{y}$

## Applications to Physics
- **Force** is a vector; forces add componentwise to give the resultant.
- **Velocity** is a vector whose magnitude is speed; velocities combine by adding vectors (e.g. a swimmer crossing a river with a current).
- **Work** counts only the force component along the motion; a perpendicular force does no work.

> [!equation]
> - **Work as a dot product:** $\displaystyle W = \vec{F}\cdot(\vec{q} - \vec{p}) = \|\vec{F}\|\,\|\vec{q} - \vec{p}\|\cos\theta$

> [!note] Connection
> See [[Newton's Laws of Motion]] (net force), [[Motion in Two and Three Dimensions]] (relative velocity) and [[Work and Kinetic Energy]].

## See Also
- [[Vectors]]
- [[Linear Transformations]]
- [[Vector Spaces]]

## Sources
- [A First Course in Linear Algebra (Kuttler), R — 4.04 Length of a Vector](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.04%3A_Length_of_a_Vector)
- [A First Course in Linear Algebra (Kuttler), R — 4.07 The Dot Product](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.07%3A_The_Dot_Product)
- [A First Course in Linear Algebra (Kuttler), R — 4.09 The Cross Product](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.09%3A_The_Cross_Product)
- [A First Course in Linear Algebra (Kuttler), R — 4.10 Spanning Linear Independence and Basis in R](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.10%3A_Spanning_Linear_Independence_and_Basis_in_R)
- [A First Course in Linear Algebra (Kuttler), R — 4.11 Orthogonality](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.11%3A_Orthogonality)
- [A First Course in Linear Algebra (Kuttler), R — 4.12 Applications](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/04%3A_R/4.12%3A_Applications)
