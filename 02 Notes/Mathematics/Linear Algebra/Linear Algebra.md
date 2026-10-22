---
aliases: [Linear Algebra Index, Matrix Algebra Index]
tags: [mathematics, linear-algebra, index]
---
# Linear Algebra

Notes on **matrix algebra, linear algebra and eigenvectors**, built from Ken Kuttler's free textbook *A First Course in Linear Algebra* (LibreTexts). These are the seven chapters that cover those topics, in the book's order. Each page links to the physics notes where the same math shows up.

> [!tip] How to read these notes
> Important equations are in pink **equation** boxes: all of a chapter's key equations at the top of its page, then each one again where it's used. Pink needs the `pink-equations` CSS snippet on.

---

## Key Equations

> [!equation] [[Systems of Linear Equations]]
> - **General linear system:** $\displaystyle \sum_{j=1}^{n} a_{ij}x_j = b_i,\quad i = 1, \ldots, m$
> - **Number of free parameters:** $\displaystyle \text{parameters} = n - \operatorname{rank}(A)$
> - **Kirchhoff loop equation:** $\displaystyle \sum R_k I_k = \sum V_k$

> [!equation] [[Matrix Algebra]]
> - **Matrix–vector product:** $\displaystyle A\vec{x} = \sum_{j=1}^{n} x_j \vec{a}_j$
> - **Size rule:** $\displaystyle (m \times n)(n \times p) = m \times p$
> - **Entry of a product:** $\displaystyle (AB)_{ij} = \sum_{k} a_{ik} b_{kj}$
> - **Transpose:** $\displaystyle (A^T)_{ij} = a_{ji}$
> - **Inverse:** $\displaystyle AA^{-1} = A^{-1}A = I$
> - **LU factorization:** $\displaystyle A = LU$

> [!equation] [[Determinants]]
> - **2×2 determinant:** $\displaystyle \det\begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc$
> - **Cofactor expansion:** $\displaystyle \det(A) = \sum_{j=1}^{n} a_{ij}\operatorname{cof}(A)_{ij}$
> - **Product rule:** $\displaystyle \det(AB) = \det(A)\det(B)$
> - **Invertibility test:** $\displaystyle A \text{ invertible} \iff \det(A) \neq 0$
> - **Inverse via adjugate:** $\displaystyle A^{-1} = \frac{1}{\det(A)}\operatorname{adj}(A)$
> - **Cramer's rule:** $\displaystyle x_i = \frac{\det(A_i)}{\det(A)}$

> [!equation] [[Vectors in Rn]]
> - **Length:** $\displaystyle \|\vec{u}\| = \sqrt{u_1^2 + \cdots + u_n^2}$
> - **Dot product:** $\displaystyle \vec{u}\cdot\vec{v} = \sum_{k=1}^{n} u_k v_k = \|\vec{u}\|\,\|\vec{v}\|\cos\theta$
> - **Projection:** $\displaystyle \operatorname{proj}_{\vec{u}}(\vec{v}) = \frac{\vec{v}\cdot\vec{u}}{\|\vec{u}\|^2}\,\vec{u}$
> - **Cross product as a determinant:** $\displaystyle \vec{u}\times\vec{v} = \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}$
> - **Linear independence:** $\displaystyle \sum_{i=1}^{k} a_i\vec{u}_i = \vec{0} \;\Rightarrow\; a_1 = \cdots = a_k = 0$
> - **Fourier expansion:** $\displaystyle \vec{x} = \sum_{j=1}^{m}\frac{\vec{x}\cdot\vec{u}_j}{\|\vec{u}_j\|^2}\,\vec{u}_j$
> - **Least squares (normal equations):** $\displaystyle A^T A\vec{x} = A^T\vec{y}$
> - **Work as a dot product:** $\displaystyle W = \vec{F}\cdot(\vec{q} - \vec{p}) = \|\vec{F}\|\,\|\vec{q} - \vec{p}\|\cos\theta$

> [!equation] [[Linear Transformations]]
> - **Linearity:** $\displaystyle T(k\vec{x}_1 + p\vec{x}_2) = kT(\vec{x}_1) + pT(\vec{x}_2)$
> - **Matrix of T:** $\displaystyle A = \begin{bmatrix} T(\vec{e}_1) & \cdots & T(\vec{e}_n) \end{bmatrix}$
> - **Rotation matrix:** $\displaystyle R_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$
> - **Dimension (rank–nullity) theorem:** $\displaystyle \dim V = \dim(\ker T) + \dim(\operatorname{im} T)$
> - **General solution:** $\displaystyle \vec{x} = \vec{x}_p + \vec{x}_0,\quad \vec{x}_0 \in \ker(T)$

> [!equation] [[Eigenvalues and Eigenvectors]]
> - **Eigenvalue equation:** $\displaystyle AX = \lambda X,\quad X \neq 0$
> - **Characteristic equation:** $\displaystyle \det(\lambda I - A) = 0$
> - **Diagonalization:** $\displaystyle A = PDP^{-1}$
> - **Powers of a matrix:** $\displaystyle A^n = PD^nP^{-1}$
> - **Matrix exponential:** $\displaystyle e^{A} = P\begin{bmatrix} e^{\lambda_1} & & \\ & \ddots & \\ & & e^{\lambda_n} \end{bmatrix}P^{-1}$
> - **Linear differential equations:** $\displaystyle X' = AX,\ X(0) = C \;\Rightarrow\; X(t) = e^{At}C$
> - **Spectral theorem:** $\displaystyle U^TAU = D,\quad U^T = U^{-1}$
> - **Singular value decomposition:** $\displaystyle A = U\Sigma V^T$

> [!equation] [[Vector Spaces]]
> - **Closure under linear combinations:** $\displaystyle a\vec{v} + b\vec{w} \in V$
> - **Dimension of polynomial spaces:** $\displaystyle \dim\mathbb{P}_2 = 3,\quad \dim\mathbb{P}_3 = 4$
> - **Matrix of T relative to bases:** $\displaystyle C_{B_2}[T(\vec{v})] = M_{B_2B_1}(T)\,C_{B_1}(\vec{v})$

---

## Chapters

1. [[Systems of Linear Equations]] — what solutions look like; elementary operations; Gaussian elimination; rank; homogeneous systems; applications.
2. [[Matrix Algebra]] — matrix arithmetic; multiplication; transpose; identity and inverses; elementary matrices; LU factorization.
3. [[Determinants]] — 2×2 and cofactor expansion; how row operations change it; det(AB); invertibility; adjugate inverse; Cramer's rule; interpolation.
4. [[Vectors in Rn]] — vectors and length; dot and cross products; span, independence and basis; orthogonality, Gram–Schmidt and least squares; physics applications.
5. [[Linear Transformations]] — linear maps as matrices; composition; rotations and reflections; one-to-one and onto; kernel and image; general solution.
6. [[Eigenvalues and Eigenvectors]] — eigenvalues and eigenvectors; characteristic equation; diagonalization; powers, Markov chains, dynamical systems and differential equations; symmetric matrices and SVD.
7. [[Vector Spaces]] — the vector space axioms; polynomials, matrices and functions as vectors; subspaces, basis and dimension; matrices of linear maps.

## How This Connects to Physics

| Idea | Linear algebra | Physics notes |
| --- | --- | --- |
| Circuits | [[Systems of Linear Equations]] solves Kirchhoff loop equations | [[Direct-Current Circuits]] |
| Dimensional analysis | [[Systems of Linear Equations]] finds the Reynolds and Mach numbers | [[Units and Measurement]], [[Fluid Mechanics]], [[Sound]] |
| Vectors, work, forces | [[Vectors in Rn]] — dot product, projection, work | [[Vectors]], [[Work and Kinetic Energy]], [[Newton's Laws of Motion]] |
| Cross product | [[Vectors in Rn]], [[Determinants]] | [[Fixed-Axis Rotation]], [[Angular Momentum]], [[Magnetic Forces and Fields]] |
| Rotation | [[Linear Transformations]] — rotation matrices | [[Motion in Two and Three Dimensions]], [[Fixed-Axis Rotation]] |
| Changing reference frames | [[Linear Transformations]] | [[Relativity]] (Lorentz transformation) |
| Oscillation | [[Eigenvalues and Eigenvectors]] — complex eigenvalues | [[Oscillations]], [[Inductance]] |
| Quantum states | [[Eigenvalues and Eigenvectors]], [[Vector Spaces]] | [[Quantum Mechanics]], [[Atomic Structure]] |
| Superposition | [[Vector Spaces]] | [[Waves]] |

## Sources
- [A First Course in Linear Algebra (Kuttler) — LibreTexts](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler))
- Each chapter page lists the sections it was built from.
