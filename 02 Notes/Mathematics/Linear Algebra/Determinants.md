---
aliases: [Determinant, Cofactor Expansion, Cramer's Rule, Adjugate]
tags: [mathematics, linear-algebra]
book-chapter: 3
---
# Determinants

> [!info] [[Linear Algebra]] › Kuttler Ch. 3: Determinants
> ← [[Matrix Algebra]] · Next: [[Vectors in Rn]] →

The **determinant** is a single number computed from a square matrix. It tells you whether the matrix is invertible, and it gives formulas for inverses and solutions.

## Key Equations

> [!equation]
> - **2×2 determinant:** $\displaystyle \det\begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc$
> - **Cofactor:** $\displaystyle \operatorname{cof}(A)_{ij} = (-1)^{i+j}\operatorname{minor}(A)_{ij}$
> - **Cofactor expansion:** $\displaystyle \det(A) = \sum_{j=1}^{n} a_{ij}\operatorname{cof}(A)_{ij}$
> - **Triangular matrix:** $\displaystyle \det(A) = a_{11}a_{22}\cdots a_{nn}$
> - **Product rule:** $\displaystyle \det(AB) = \det(A)\det(B)$
> - **Transpose:** $\displaystyle \det(A^T) = \det(A)$
> - **Scalar multiple:** $\displaystyle \det(kA) = k^n\det(A)$
> - **Invertibility test:** $\displaystyle A \text{ invertible} \iff \det(A) \neq 0$
> - **Determinant of the inverse:** $\displaystyle \det(A^{-1}) = \frac{1}{\det(A)}$
> - **Inverse via adjugate:** $\displaystyle A^{-1} = \frac{1}{\det(A)}\operatorname{adj}(A)$
> - **2×2 adjugate:** $\displaystyle \operatorname{adj}\begin{bmatrix} a & b \\ c & d \end{bmatrix} = \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$
> - **Cramer's rule:** $\displaystyle x_i = \frac{\det(A_i)}{\det(A)}$

---

## Basic Techniques
- The **minor** $\text{minor}(A)_{ij}$ is the determinant left after deleting row $i$ and column $j$; the **cofactor** adds a sign.
- **Cofactor (Laplace) expansion:** multiply each entry of any row or column by its cofactor and add — every row or column gives the same answer.
- For a triangular matrix, the determinant is the product of the diagonal entries.

> [!equation]
> - **2×2 determinant:** $\displaystyle \det\begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc$
> - **Cofactor:** $\displaystyle \operatorname{cof}(A)_{ij} = (-1)^{i+j}\operatorname{minor}(A)_{ij}$
> - **Cofactor expansion:** $\displaystyle \det(A) = \sum_{j=1}^{n} a_{ij}\operatorname{cof}(A)_{ij}$
> - **Triangular matrix:** $\displaystyle \det(A) = a_{11}a_{22}\cdots a_{nn}$

> [!note] Connection
> The cross product is computed as a 3×3 determinant — see [[Vectors in Rn]].

## Properties of Determinants
- Swapping two rows flips the sign; multiplying a row by $k$ multiplies the determinant by $k$; adding a multiple of one row to another changes nothing.
- So a determinant can be found by row-reducing to triangular form and tracking these changes.

> [!equation]
> - **Product rule:** $\displaystyle \det(AB) = \det(A)\det(B)$
> - **Transpose:** $\displaystyle \det(A^T) = \det(A)$
> - **Scalar multiple:** $\displaystyle \det(kA) = k^n\det(A)$
> - **Invertibility test:** $\displaystyle A \text{ invertible} \iff \det(A) \neq 0$
> - **Determinant of the inverse:** $\displaystyle \det(A^{-1}) = \frac{1}{\det(A)}$

## Applications of the Determinant
- The **adjugate** is the transpose of the cofactor matrix; it gives a formula for the inverse.
- **Cramer's rule** solves an invertible square system one variable at a time: replace column $i$ with $\vec{b}$.
- **Polynomial interpolation:** $n$ points with distinct $x$-values determine a unique polynomial of degree $n-1$, found by solving a linear system.

> [!equation]
> - **Inverse via adjugate:** $\displaystyle A^{-1} = \frac{1}{\det(A)}\operatorname{adj}(A)$
> - **2×2 adjugate:** $\displaystyle \operatorname{adj}\begin{bmatrix} a & b \\ c & d \end{bmatrix} = \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$
> - **Cramer's rule:** $\displaystyle x_i = \frac{\det(A_i)}{\det(A)}$

> [!note] Connection
> Cramer's rule is a quick way to solve the small loop-current systems from [[Direct-Current Circuits]] (see [[Systems of Linear Equations]]).

## See Also
- [[Matrix Algebra]]
- [[Eigenvalues and Eigenvectors]]
- [[Vectors in Rn]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Determinants — 3.01 Basic Techniques](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/03%3A_Determinants/3.01%3A_Basic_Techniques)
- [A First Course in Linear Algebra (Kuttler), Determinants — 3.02 Properties of Determinants](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/03%3A_Determinants/3.02%3A_Properties_of_Determinants)
- [A First Course in Linear Algebra (Kuttler), Determinants — 3.04 Applications of the Determinant](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/03%3A_Determinants/3.04%3A_Applications_of_the_Determinant)
