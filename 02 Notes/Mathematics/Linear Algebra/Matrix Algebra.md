---
aliases: [Matrices, Matrix Multiplication, Matrix Inverse, Transpose, LU Factorization]
tags: [mathematics, linear-algebra]
book-chapter: 2
---
# Matrix Algebra

> [!info] [[Linear Algebra]] › Kuttler Ch. 2: Matrices
> ← [[Systems of Linear Equations]] · Next: [[Determinants]] →

**Matrix algebra** treats a whole table of numbers as a single object you can add, multiply and invert. It turns any linear system into the compact form $A\vec{x} = \vec{b}$.

## Key Equations

> [!equation]
> - **Addition:** $\displaystyle (A + B)_{ij} = a_{ij} + b_{ij}$
> - **Scalar multiplication:** $\displaystyle (kA)_{ij} = k\,a_{ij}$
> - **Matrix–vector product:** $\displaystyle A\vec{x} = \sum_{j=1}^{n} x_j \vec{a}_j$
> - **Size rule:** $\displaystyle (m \times n)(n \times p) = m \times p$
> - **Entry of a product:** $\displaystyle (AB)_{ij} = \sum_{k} a_{ik} b_{kj}$
> - **Associative:** $\displaystyle A(BC) = (AB)C$
> - **Distributive:** $\displaystyle A(rB + sC) = r(AB) + s(AC)$
> - **Transpose:** $\displaystyle (A^T)_{ij} = a_{ji}$
> - **Transpose of a product:** $\displaystyle (AB)^T = B^T A^T$
> - **Inverse:** $\displaystyle AA^{-1} = A^{-1}A = I$
> - **Inversion algorithm:** $\displaystyle [A \mid I] \rightarrow [I \mid A^{-1}]$
> - **LU factorization:** $\displaystyle A = LU$

---

## Matrix Arithmetic
- Matrices of the **same size** add entry by entry; scalar multiplication multiplies every entry.
- Addition is commutative and associative, with the zero matrix as identity.

> [!equation]
> - **Addition:** $\displaystyle (A + B)_{ij} = a_{ij} + b_{ij}$
> - **Scalar multiplication:** $\displaystyle (kA)_{ij} = k\,a_{ij}$

## Matrix Multiplication
- An $n \times 1$ matrix is a **column vector**. $A\vec{x}$ is a combination of the columns of $A$ weighted by the entries of $\vec{x}$.
- $AB$ is defined only when the columns of $A$ match the rows of $B$.
- Any linear system can be written $A\vec{x} = \vec{b}$.

> [!equation]
> - **Matrix–vector product:** $\displaystyle A\vec{x} = \sum_{j=1}^{n} x_j \vec{a}_j$
> - **Size rule:** $\displaystyle (m \times n)(n \times p) = m \times p$
> - **Entry of a product:** $\displaystyle (AB)_{ij} = \sum_{k} a_{ik} b_{kj}$

## Properties of Multiplication
- Multiplication is **associative** and **distributive**, but **not commutative**: in general $AB \neq BA$, even when both exist.

> [!equation]
> - **Associative:** $\displaystyle A(BC) = (AB)C$
> - **Distributive:** $\displaystyle A(rB + sC) = r(AB) + s(AC)$

> [!note] Connection
> Order matters the same way it does for the cross product, where $\vec{A}\times\vec{B} = -\vec{B}\times\vec{A}$ — see [[Vectors]].

## The Transpose
- The **transpose** swaps rows and columns.
- $A$ is **symmetric** if $A = A^T$ and **skew-symmetric** if $A = -A^T$.

> [!equation]
> - **Transpose:** $\displaystyle (A^T)_{ij} = a_{ji}$
> - **Transpose of a product:** $\displaystyle (AB)^T = B^T A^T$

## Identity and Inverses
- The **identity** $I$ has 1s on the diagonal and 0s elsewhere; $AI = IA = A$.
- A square matrix is **invertible** if some $A^{-1}$ gives $AA^{-1} = A^{-1}A = I$; the inverse is unique.
- Find it by row reducing $[A \mid I]$ to $[I \mid A^{-1}]$; if the left side can't reach $I$, there is no inverse.

> [!equation]
> - **Inverse:** $\displaystyle AA^{-1} = A^{-1}A = I$
> - **Inversion algorithm:** $\displaystyle [A \mid I] \rightarrow [I \mid A^{-1}]$

> [!note] Connection
> A determinant test for invertibility is in [[Determinants]].

## Elementary Matrices
- An **elementary matrix** is the identity after one row operation; multiplying $EA$ performs that row operation on $A$.
- Every elementary matrix is invertible.
- A square matrix is invertible exactly when it is a product of elementary matrices.

## LU Factorization
- Write $A = LU$: $L$ lower triangular with 1s on the diagonal, $U$ upper triangular.
- It exists when $A$ can be row-reduced without swapping rows.
- To solve $A\vec{x} = \vec{b}$: solve $L\vec{y} = \vec{b}$, then $U\vec{x} = \vec{y}$ — both quick because they are triangular.

> [!equation]
> - **LU factorization:** $\displaystyle A = LU$

## See Also
- [[Systems of Linear Equations]]
- [[Determinants]]
- [[Linear Transformations]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.01 Matrix Arithmetic](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.01%3A_Matrix_Arithmetic)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.02 Multiplication of Matrices](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.02%3A_Multiplication_of_Matrices)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.04 Properties of Matrix Multiplication](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.04%3A_Properties_of_Matrix_Multiplication)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.05 The Transpose](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.05%3A_The_Transpose)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.06  The Identity and Inverses](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.06%3A__The_Identity_and_Inverses)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.07 Finding the Inverse of a Matrix](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.07%3A_Finding_the_Inverse_of_a_Matrix)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.08 Elementary Matrices](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.08%3A_Elementary_Matrices)
- [A First Course in Linear Algebra (Kuttler), Matrices — 2.10 LU Factorization](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/02%3A_Matrices/2.10%3A_LU_Factorization)
