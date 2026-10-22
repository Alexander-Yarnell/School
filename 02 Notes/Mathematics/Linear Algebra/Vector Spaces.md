---
aliases: [Vector Space, Subspace, Coordinate Vector, Function Space]
tags: [mathematics, linear-algebra]
book-chapter: 9
---
# Vector Spaces

> [!info] [[Linear Algebra]] › Kuttler Ch. 9: Vector Spaces
> ← [[Eigenvalues and Eigenvectors]]

A **vector space** is any collection you can add and scale following the same rules as arrows. Polynomials, matrices and even functions qualify, so everything in linear algebra applies to them too.

## Key Equations

> [!equation]
> - **Closure under linear combinations:** $\displaystyle a\vec{v} + b\vec{w} \in V$
> - **Functions as vectors:** $\displaystyle (f + g)(x) = f(x) + g(x),\quad (af)(x) = a\,f(x)$
> - **Dimension of polynomial spaces:** $\displaystyle \dim\mathbb{P}_2 = 3,\quad \dim\mathbb{P}_3 = 4$
> - **Matrix of T relative to bases:** $\displaystyle C_{B_2}[T(\vec{v})] = M_{B_2B_1}(T)\,C_{B_1}(\vec{v})$
> - **Composition:** $\displaystyle M_{B_3B_1}(ST) = M_{B_3B_2}(S)\,M_{B_2B_1}(T)$

---

## The Vector Space Axioms
- A vector space is a set with addition and scalar multiplication that are closed, commutative and associative, have a zero vector and additive inverses, distribute, and satisfy $1\vec{v} = \vec{v}$.
- Examples: $\mathbb{R}^n$; polynomials $\mathbb{P}_n$; $m \times n$ matrices $\mathbb{M}_{m,n}$; real functions on a set, added and scaled pointwise.
- In any vector space, $0\vec{x} = \vec{0}$ and $(-1)\vec{x} = -\vec{x}$.

> [!equation]
> - **Closure under linear combinations:** $\displaystyle a\vec{v} + b\vec{w} \in V$
> - **Functions as vectors:** $\displaystyle (f + g)(x) = f(x) + g(x),\quad (af)(x) = a\,f(x)$

> [!note] Connection
> Because the [[Waves|wave equation]] is linear, adding two solutions gives another — wave superposition is the statement that solutions form a vector space. Wave functions in [[Quantum Mechanics]] are combined the same way.

## Subspaces, Basis and Dimension
- **Subspace test:** contains $\vec 0$, closed under addition and scalar multiplication.
- A **basis** spans and is independent; the **dimension** is its size.
- $\{1, x, x^2\}$ is a basis of $\mathbb{P}_2$, so $\dim\mathbb{P}_2 = 3$; $\dim\mathbb{P}_3 = 4$.

> [!equation]
> - **Dimension of polynomial spaces:** $\displaystyle \dim\mathbb{P}_2 = 3,\quad \dim\mathbb{P}_3 = 4$

> [!note] Connection
> Same definitions as in $\mathbb{R}^n$ — see [[Vectors in Rn]].

## The Matrix of a Linear Transformation
- Choosing a basis $B$ turns each vector into a **coordinate vector** $C_B(\vec{v})$ in $\mathbb{R}^n$; the order of the basis matters.
- Any linear map between finite-dimensional spaces then becomes a matrix, and composition becomes matrix multiplication.
- $T$ is an isomorphism exactly when its matrix is invertible.

> [!equation]
> - **Matrix of T relative to bases:** $\displaystyle C_{B_2}[T(\vec{v})] = M_{B_2B_1}(T)\,C_{B_1}(\vec{v})$
> - **Composition:** $\displaystyle M_{B_3B_1}(ST) = M_{B_3B_2}(S)\,M_{B_2B_1}(T)$

> [!note] Connection
> This generalizes the standard-basis matrix in [[Linear Transformations]].

## See Also
- [[Vectors in Rn]]
- [[Linear Transformations]]
- [[Quantum Mechanics]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Vector Spaces — 9.01 Algebraic Considerations](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/09%3A_Vector_Spaces/9.01%3A_Algebraic_Considerations)
- [A First Course in Linear Algebra (Kuttler), Vector Spaces — 9.04 Subspaces and Basis](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/09%3A_Vector_Spaces/9.04%3A_Subspaces_and_Basis)
- [A First Course in Linear Algebra (Kuttler), Vector Spaces — 9.09 The Matrix of a Linear Transformation](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/09%3A_Vector_Spaces/9.09%3A_The_Matrix_of_a_Linear_Transformation)
