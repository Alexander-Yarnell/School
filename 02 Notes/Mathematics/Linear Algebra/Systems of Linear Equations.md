---
aliases: [Gaussian Elimination, Row Reduction, Row-Echelon Form, RREF, Rank]
tags: [mathematics, linear-algebra]
book-chapter: 1
---
# Systems of Linear Equations

> [!info] [[Linear Algebra]] › Kuttler Ch. 1: Systems of Equations
> Next: [[Matrix Algebra]] →

**Systems of linear equations** are the starting point of linear algebra: several linear equations in several unknowns, solved by row-reducing a matrix.

## Key Equations

> [!equation]
> - **General linear system:** $\displaystyle \sum_{j=1}^{n} a_{ij}x_j = b_i,\quad i = 1, \ldots, m$
> - **Augmented matrix:** $\displaystyle \left[\begin{array}{ccc|c} a_{11} & \cdots & a_{1n} & b_1 \\ \vdots & & \vdots & \vdots \\ a_{m1} & \cdots & a_{mn} & b_m \end{array}\right]$
> - **Number of free parameters:** $\displaystyle \text{parameters} = n - \operatorname{rank}(A)$
> - **Rank and consistent systems:** $\displaystyle r = n \Rightarrow \text{unique solution},\qquad r < n \Rightarrow n - r \text{ parameters}$
> - **Mach number:** $\displaystyle \mathcal{M} = \frac{V}{V_0}$
> - **Reynolds number:** $\displaystyle Re = \frac{AV\rho}{\mu}$
> - **Kirchhoff loop equation:** $\displaystyle \sum R_k I_k = \sum V_k$

---

## Geometry of Solutions
- A linear system always has **exactly one**, **infinitely many**, or **no** solutions.
- Two lines meet at a point, are parallel (none) or coincide (infinitely many). Two planes in 3D can't meet at just one point — they meet in a line or not at all.

## Systems and Elementary Operations
- A system has $m$ equations in $n$ variables; it is **consistent** if it has a solution, **inconsistent** if not.
- **Elementary operations:** swap two equations; multiply one by a nonzero number; add a multiple of one equation to another.
- Elementary operations never change the solution set.

> [!equation]
> - **General linear system:** $\displaystyle \sum_{j=1}^{n} a_{ij}x_j = b_i,\quad i = 1, \ldots, m$

## Gaussian Elimination
- Write the system as an **augmented matrix** and use **row operations** (the same three operations, on rows).
- **Row-echelon form:** zero rows at the bottom, each leading entry to the right of the one above, leading entries equal to 1. **Reduced** row-echelon form also has zeros above and below every leading 1.
- A leading entry's position is a **pivot position**; its column is a **pivot column**.
- **Gaussian elimination** stops at row-echelon form and back-substitutes; **Gauss–Jordan** continues to reduced form.
- Reading the result: a row $[0 \cdots 0 \mid 1]$ means no solution; every coefficient column a pivot means one solution; otherwise, non-pivot variables become free parameters (infinitely many).

> [!equation]
> - **Augmented matrix:** $\displaystyle \left[\begin{array}{ccc|c} a_{11} & \cdots & a_{1n} & b_1 \\ \vdots & & \vdots & \vdots \\ a_{m1} & \cdots & a_{mn} & b_m \end{array}\right]$

## Rank and Homogeneous Systems
- A **homogeneous** system has every right-hand side 0; it always has the **trivial** solution $x = 0$.
- The **rank** of a matrix is its number of pivot positions.
- More variables than equations ($n > m$) in a homogeneous system ⇒ infinitely many solutions.
- Any linear combination of the **basic solutions** of a homogeneous system is again a solution.

> [!equation]
> - **Number of free parameters:** $\displaystyle \text{parameters} = n - \operatorname{rank}(A)$
> - **Rank and consistent systems:** $\displaystyle r = n \Rightarrow \text{unique solution},\qquad r < n \Rightarrow n - r \text{ parameters}$

## Application: Dimensionless Variables
- To find dimensionless groups for wing lift, write each group as a product of powers of the variables and require the exponents of meters, seconds and kilograms to cancel — a homogeneous linear system.
- Its four basic solutions give the aspect ratio, the angle, the **Mach number** and the **Reynolds number**.

> [!equation]
> - **Mach number:** $\displaystyle \mathcal{M} = \frac{V}{V_0}$
> - **Reynolds number:** $\displaystyle Re = \frac{AV\rho}{\mu}$

> [!note] Connection
> This is [[Units and Measurement|dimensional analysis]] turned into a linear system. The Reynolds number also decides laminar vs turbulent flow in [[Fluid Mechanics]], and the Mach number appears with shock waves in [[Sound]].

## Application: Resistor Networks
- Each loop of a circuit gives one equation: around a loop, the sum of resistance × current equals the sum of the voltage sources.
- A resistor shared by two loops carries the difference of the two loop currents.
- The loop equations form $A\vec{x} = \vec{b}$, solved by Gaussian elimination; a negative current means it flows clockwise.

> [!equation]
> - **Kirchhoff loop equation:** $\displaystyle \sum R_k I_k = \sum V_k$

> [!note] Connection
> This is Kirchhoff's loop rule and Ohm's law ($V = IR$) from [[Direct-Current Circuits]] and [[Current and Resistance]] — linear algebra is how larger circuits are actually solved.

## See Also
- [[Matrix Algebra]]
- [[Determinants]]
- [[Direct-Current Circuits]]

## Sources
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.01 Geometry](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.01%3A_Geometry)
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.02 Elementary Operations](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.02%3A_Elementary_Operations)
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.03 Gaussian Elimination](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.03%3A_Gaussian_Elimination)
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.05 Rank and Homogeneous Systems](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.05%3A_Rank_and_Homogeneous_Systems)
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.07 Dimensionless Variables](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.07%3A_Dimensionless_Variables)
- [A First Course in Linear Algebra (Kuttler), Systems of Equations — 1.08 An Application to Resistor Networks](https://math.libretexts.org/Bookshelves/Linear_Algebra/A_First_Course_in_Linear_Algebra_(Kuttler)/01%3A_Systems_of_Equations/1.08%3A_An_Application_to_Resistor_Networks)
