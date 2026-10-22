---
aliases: [Eigenvalue, Eigenvector, Eigenvectors, Spectral Theory, Diagonalization, Characteristic Equation, Spectral Theorem, SVD]
tags: [mathematics, linear-algebra]
book-chapter: 7
---
# Eigenvalues and Eigenvectors

> [!info] [[Linear Algebra]] › Kuttler Ch. 7: Spectral Theory
> ← [[Linear Transformations]] · Next: [[Vector Spaces]] →

An **eigenvector** of a matrix is a direction the matrix only stretches — it doesn't turn it. The stretch factor is the **eigenvalue**. Kuttler calls this topic **spectral theory**, and it is the key to powers of matrices, dynamical systems and differential equations.

## Key Equations

> [!equation]
> - **Eigenvalue equation:** $\displaystyle AX = \lambda X,\quad X \neq 0$
> - **Characteristic equation:** $\displaystyle \det(\lambda I - A) = 0$
> - **Eigenvector system:** $\displaystyle (\lambda I - A)X = 0$
> - **Similar matrices:** $\displaystyle A = P^{-1}BP$
> - **Diagonalization:** $\displaystyle A = PDP^{-1}$
> - **Eigenspace:** $\displaystyle E_\lambda(A) = \operatorname{null}(\lambda I - A)$
> - **Powers of a matrix:** $\displaystyle A^n = PD^nP^{-1}$
> - **Markov steady state:** $\displaystyle AX_s = X_s$
> - **Dynamical system:** $\displaystyle V_n = PD^nP^{-1}V_0$
> - **Matrix exponential:** $\displaystyle e^{A} = P\begin{bmatrix} e^{\lambda_1} & & \\ & \ddots & \\ & & e^{\lambda_n} \end{bmatrix}P^{-1}$
> - **Linear differential equations:** $\displaystyle X' = AX,\ X(0) = C \;\Rightarrow\; X(t) = e^{At}C$
> - **Spectral theorem:** $\displaystyle U^TAU = D,\quad U^T = U^{-1}$
> - **Determinant and trace:** $\displaystyle \det(A) = \prod \lambda_i,\qquad \operatorname{tr}(A) = \sum \lambda_i$
> - **Positive definite:** $\displaystyle \vec{x}^TA\vec{x} > 0 \text{ for all } \vec{x} \neq \vec{0}$
> - **Singular value decomposition:** $\displaystyle A = U\Sigma V^T$

---

## Eigenvalues and Eigenvectors
- $\lambda$ is an **eigenvalue** and $X \neq 0$ an **eigenvector** if $AX = \lambda X$. The set of eigenvalues is the **spectrum**.
- Eigenvectors can never be $\vec 0$, but an eigenvalue can be 0.
- **Procedure:** solve $\det(\lambda I - A) = 0$ for $\lambda$; for each, solve $(\lambda I - A)X = 0$ for the basic eigenvectors; check $AX = \lambda X$.
- The **multiplicity** of $\lambda$ is how many times it is a root of the characteristic polynomial.
- The eigenvalues of a triangular matrix are its diagonal entries.
- **Similar** matrices ($A = P^{-1}BP$) have the same eigenvalues.

> [!equation]
> - **Eigenvalue equation:** $\displaystyle AX = \lambda X,\quad X \neq 0$
> - **Characteristic equation:** $\displaystyle \det(\lambda I - A) = 0$
> - **Eigenvector system:** $\displaystyle (\lambda I - A)X = 0$
> - **Similar matrices:** $\displaystyle A = P^{-1}BP$

> [!note] Connection
> The time-independent Schrödinger equation in [[Quantum Mechanics]], $-\frac{\hbar^2}{2m}\psi'' + U\psi = E\psi$, has exactly this shape: an operator acting on $\psi$ returns $\psi$ times a number. The allowed energies $E_n$ are its eigenvalues and the stationary states $\psi_n$ are its eigenvectors.

## Diagonalization
- $A$ is **diagonalizable** if $P^{-1}AP = D$ is diagonal. The columns of $P$ are eigenvectors and the diagonal of $D$ holds the eigenvalues, in the same order.
- This works exactly when $A$ has $n$ independent eigenvectors — guaranteed if it has $n$ distinct eigenvalues.
- Each eigenspace's dimension must equal the eigenvalue's multiplicity; $\begin{bmatrix}1&1\\0&1\end{bmatrix}$ fails.
- Real matrices can have complex eigenvalues, which come in conjugate pairs.

> [!equation]
> - **Diagonalization:** $\displaystyle A = PDP^{-1}$
> - **Eigenspace:** $\displaystyle E_\lambda(A) = \operatorname{null}(\lambda I - A)$

## Applications
- **Powers:** diagonalizing makes $A^n$ easy — raise each eigenvalue to the $n$th power.
- **Markov (migration) matrices** have nonnegative entries and columns summing to 1; $\lambda = 1$ is always an eigenvalue and the **steady state** is its eigenvector.
- **Discrete dynamical systems** $V_{n+1} = AV_n$: if every $|\lambda| < 1$ the solution shrinks to the origin; any $|\lambda| > 1$ makes it generally grow without bound. Complex eigenvalues make solutions **spiral**.
- The Fibonacci numbers come from the eigenvalues of $\begin{bmatrix}0&1\\1&1\end{bmatrix}$.
- **Differential equations:** $X' = AX$ is solved with the matrix exponential, built from the eigenvalues.
- Predator–prey (Lotka–Volterra) models linearized near equilibrium have complex eigenvalues, giving spirals.

> [!equation]
> - **Powers of a matrix:** $\displaystyle A^n = PD^nP^{-1}$
> - **Markov steady state:** $\displaystyle AX_s = X_s$
> - **Dynamical system:** $\displaystyle V_n = PD^nP^{-1}V_0$
> - **Matrix exponential:** $\displaystyle e^{A} = P\begin{bmatrix} e^{\lambda_1} & & \\ & \ddots & \\ & & e^{\lambda_n} \end{bmatrix}P^{-1}$
> - **Linear differential equations:** $\displaystyle X' = AX,\ X(0) = C \;\Rightarrow\; X(t) = e^{At}C$

> [!note] Connection
> A mass on a spring, $x'' = -\frac{k}{m}x$ ([[Oscillations]]), can be written as $X' = AX$ with $X = (x, v)$ and $A = \begin{bmatrix}0 & 1\\ -k/m & 0\end{bmatrix}$. Solving $\det(\lambda I - A) = 0$ gives $\lambda = \pm i\sqrt{k/m} = \pm i\omega$ — complex eigenvalues, so the motion oscillates at $\omega = \sqrt{k/m}$. The same holds for LC circuits in [[Inductance]].

## Symmetric Matrices and Orthogonality
- A real **symmetric** matrix has real eigenvalues, and eigenvectors for different eigenvalues are orthogonal.
- **Spectral (principal axis) theorem:** a symmetric matrix can be diagonalized by an orthogonal matrix; its orthonormal eigenvectors are the **principal axes**.
- $\det(A)$ is the product of the eigenvalues; the trace is their sum.
- **Positive definite:** symmetric with all eigenvalues positive, i.e. $\vec{x}^TA\vec{x} > 0$ for every nonzero $\vec{x}$.
- **Singular value decomposition:** any matrix factors as $U\Sigma V^T$; the singular values are the square roots of the positive eigenvalues of $A^TA$.

> [!equation]
> - **Spectral theorem:** $\displaystyle U^TAU = D,\quad U^T = U^{-1}$
> - **Determinant and trace:** $\displaystyle \det(A) = \prod \lambda_i,\qquad \operatorname{tr}(A) = \sum \lambda_i$
> - **Positive definite:** $\displaystyle \vec{x}^TA\vec{x} > 0 \text{ for all } \vec{x} \neq \vec{0}$
> - **Singular value decomposition:** $\displaystyle A = U\Sigma V^T$

## See Also
- [[Matrix Algebra]]
- [[Determinants]]
- [[Quantum Mechanics]]
- [[Oscillations]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Spectral Theory — 7.01 Eigenvalues and Eigenvectors of a Matrix](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/07%3A_Spectral_Theory/7.01%3A_Eigenvalues_and_Eigenvectors_of_a_Matrix)
- [A First Course in Linear Algebra (Kuttler), Spectral Theory — 7.02 Diagonalization](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/07%3A_Spectral_Theory/7.02%3A_Diagonalization)
- [A First Course in Linear Algebra (Kuttler), Spectral Theory — 7.03 Applications of Spectral Theory](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/07%3A_Spectral_Theory/7.03%3A_Applications_of_Spectral_Theory)
- [A First Course in Linear Algebra (Kuttler), Spectral Theory — 7.04 Orthogonality](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/07%3A_Spectral_Theory/7.04%3A_Orthogonality)
