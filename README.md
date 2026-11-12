# GTU Maths 2 diagonalization checker (eigenvalues, AM vs GM, P and D)

For GTU BE Mathematics 2 (BE02000011), whose matrices unit includes eigenvalues, eigenvectors and diagonalization, as summarised in GTU Hero's Maths 2 guide. 2×2 ya 3×3 matrix daalo: ye page characteristic polynomial ke roots, algebraic and geometric multiplicity, and agar diagonalizable hai toh P aur D deta hai, with a P⁻¹AP check.

Live page: https://princeadvant.github.io/gtu-maths-2-diagonalization-checker/

## Formulas

- Characteristic equation: det(A − λI) = 0
- For 3×3: λ³ − (trace) λ² + (sum of principal 2×2 minors) λ − det A = 0
- Algebraic multiplicity (AM) = times λ repeats; geometric multiplicity (GM) = n − rank(A − λI)
- A is diagonalizable iff GM = AM for every eigenvalue; then P⁻¹AP = D

## Test

`node test.js` checks the formulas against hand-worked values and prints `All checks passed`.

## Tips

- Default matrix is own practice (not from a GTU paper): eigenvalues 1, 1, 4. λ = 1 repeats but A − I has rank 1, so GM = 2 = AM and it IS diagonalizable.
- Try 2 0 0; 1 2 0; 0 0 3: λ = 2 repeats but GM = 1, so not diagonalizable. Repeated root dekhte hi rank check karo.
- Shortcut check: sum of eigenvalues = trace, product = det. Exam mein 10 second ka self-check.

Old papers by subject code and session: [GTU Hero question papers](https://gtuhero.com/gtu-papers) (GTU Hero is my project).
