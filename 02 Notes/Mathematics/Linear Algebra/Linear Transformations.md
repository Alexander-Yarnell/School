---
aliases: [Linear Transformation, Linear Map, Rotation Matrix, Kernel, Image, Rank-Nullity]
tags: [mathematics, linear-algebra]
book-chapter: 5
---
# Linear Transformations

> [!info] [[Linear Algebra]] › Kuttler Ch. 5: Linear Transformations
> ← [[Vectors in Rn]] · Next: [[Eigenvalues and Eigenvectors]] →

A **linear transformation** is a function that respects addition and scaling. Every one of them is multiplication by a matrix, so matrices *are* linear transformations — rotations, reflections and projections included.

## Key Equations

> [!equation]
> - **Linearity:** $\displaystyle T(k\vec{x}_1 + p\vec{x}_2) = kT(\vec{x}_1) + pT(\vec{x}_2)$
> - **Matrix of T:** $\displaystyle A = \begin{bmatrix} T(\vec{e}_1) & \cdots & T(\vec{e}_n) \end{bmatrix}$
> - **Composition:** $\displaystyle (S \circ T)(\vec{x}) = BA\,\vec{x}$
> - **Rotation matrix:** $\displaystyle R_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$
> - **Composition of rotations:** $\displaystyle R_{\theta+\phi} = R_\theta R_\phi$
> - **Reflection across y = mx:** $\displaystyle Q_m = \frac{1}{1+m^2}\begin{bmatrix} 1-m^2 & 2m \\ 2m & m^2-1 \end{bmatrix}$
> - **One-to-one test:** $\displaystyle \operatorname{rank}(A) = n$
> - **Onto test:** $\displaystyle \operatorname{rank}(A) = m$
> - **Kernel:** $\displaystyle \ker(T) = \{\vec{v} : T(\vec{v}) = \vec{0}\}$
> - **Dimension (rank–nullity) theorem:** $\displaystyle \dim V = \dim(\ker T) + \dim(\operatorname{im} T)$
> - **General solution:** $\displaystyle \vec{x} = \vec{x}_p + \vec{x}_0,\quad \vec{x}_0 \in \ker(T)$

---

## Linear Transformations
- $T$ is linear if it preserves linear combinations.
- Every matrix transformation $T(\vec{x}) = A\vec{x}$ is linear — and every linear transformation is a matrix transformation.

> [!equation]
> - **Linearity:** $\displaystyle T(k\vec{x}_1 + p\vec{x}_2) = kT(\vec{x}_1) + pT(\vec{x}_2)$

> [!note] Connection
> The Galilean and Lorentz transformations in [[Relativity]] are linear in $(x, t)$ — changing reference frames is a linear transformation.

## The Matrix of a Linear Transformation
- The columns of the matrix are the images of the standard basis vectors.
- Linear maps send $\vec{0}$ to $\vec{0}$ and preserve negatives.

> [!equation]
> - **Matrix of T:** $\displaystyle A = \begin{bmatrix} T(\vec{e}_1) & \cdots & T(\vec{e}_n) \end{bmatrix}$

## Composition
- Doing $T$ (matrix $A$) then $S$ (matrix $B$) is the transformation with matrix $BA$ — in that order.

> [!equation]
> - **Composition:** $\displaystyle (S \circ T)(\vec{x}) = BA\,\vec{x}$

> [!note] Connection
> This is why matrix multiplication isn't commutative — see [[Matrix Algebra]].

## Rotations and Reflections in R²
- Rotating by $\theta$ is multiplication by $R_\theta$; rotating by $\phi$ then $\theta$ is a rotation by $\theta + \phi$.
- Multiplying out $R_\theta R_\phi$ gives the angle-sum trig identities.
- Reflection across the line $y = mx$ has its own matrix $Q_m$.

> [!equation]
> - **Rotation matrix:** $\displaystyle R_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$
> - **Composition of rotations:** $\displaystyle R_{\theta+\phi} = R_\theta R_\phi$
> - **Reflection across y = mx:** $\displaystyle Q_m = \frac{1}{1+m^2}\begin{bmatrix} 1-m^2 & 2m \\ 2m & m^2-1 \end{bmatrix}$

> [!note] Connection
> Uniform circular motion $\vec r(t) = A\cos\omega t\,\hat i + A\sin\omega t\,\hat j$ in [[Motion in Two and Three Dimensions]] is $R_{\omega t}$ applied to $A\hat i$ — the angle $\theta = \omega t$ from [[Fixed-Axis Rotation]].

## One-to-One and Onto
- **One-to-one:** different inputs give different outputs. **Onto:** every output is reached.
- For an $m \times n$ matrix: one-to-one ⇔ rank $n$; onto ⇔ rank $m$.

> [!equation]
> - **One-to-one test:** $\displaystyle \operatorname{rank}(A) = n$
> - **Onto test:** $\displaystyle \operatorname{rank}(A) = m$

## Kernel and Image
- The **kernel** is everything sent to $\vec 0$; the **image** is everything that comes out. Both are subspaces.
- Their dimensions add up to the dimension of the input space.

> [!equation]
> - **Kernel:** $\displaystyle \ker(T) = \{\vec{v} : T(\vec{v}) = \vec{0}\}$
> - **Dimension (rank–nullity) theorem:** $\displaystyle \dim V = \dim(\ker T) + \dim(\operatorname{im} T)$

## The General Solution of a Linear System
- Every solution of $T(\vec{x}) = \vec{b}$ is one **particular** solution plus a solution of the **homogeneous** system $T(\vec{x}) = \vec{0}$.

> [!equation]
> - **General solution:** $\displaystyle \vec{x} = \vec{x}_p + \vec{x}_0,\quad \vec{x}_0 \in \ker(T)$

> [!note] Connection
> The kernel of $\frac{d}{dx}$ is the constant functions — the same reason integrals in [[Motion Along a Straight Line]] carry a $+C$.

## See Also
- [[Matrix Algebra]]
- [[Eigenvalues and Eigenvectors]]
- [[Relativity]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.01 Linear Transformations](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.01%3A_Linear_Transformations)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.02 The Matrix of a Linear Transformation I](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.02%3A_The_Matrix_of_a_Linear_Transformation_I)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.03 Properties of Linear Transformations](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.03%3A_Properties_of_Linear_Transformations)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.04 Special Linear Transformations in R](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.04%3A_Special_Linear_Transformations_in_R)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.05 One-to-One and Onto Transformations](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.05%3A_One-to-One_and_Onto_Transformations)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.07 The Kernel and Image of A Linear Map](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.07%3A_The_Kernel_and_Image_of_A_Linear_Map)
- [A First Course in Linear Algebra (Kuttler), Linear Transformations — 5.09 The General Solution of a Linear System](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/05%3A_Linear_Transformations/5.09%3A_The_General_Solution_of_a_Linear_System)
