Algorithm:

---

### 1. **Recursion and Dynamic Programming**
- Break the problem into smaller subproblems (e.g., tiling a 2×n board with dominoes).
- Set up a recurrence relation based on the first tile placed.
- Example:  
  Let f(n) = number of ways to tile a 2×n board with 2×1 dominoes.  
  f(n) = f(n-1) + f(n-2)

---

### 2. **Coloring and Parity Arguments**
- Use coloring (checkerboard, etc.) to show impossibility or count configurations.
- Parity (odd/even) arguments often reveal constraints (e.g., domino covers one black and one white square).

---

### 3. **Invariants**
- Identify a property that remains unchanged after each move or placement.
- Useful for proving impossibility or uniqueness.

---

### 4. **Generating Functions**
- Encode the number of ways to tile or cover as coefficients in a generating function.
- Useful for more complex recurrences.

---

### 5. **Graph Theory**
- Model the problem as a matching in a graph (e.g., perfect matchings for domino tilings).
- Use Hall’s Marriage Theorem or other matching results.

---

### 6. **Symmetry and Casework**
- Consider symmetries to reduce the number of cases.
- Use casework for small boards or when certain placements force others.

---

### 7. **Constructive Algorithms**
- Explicitly construct a tiling or covering to show existence.
- Sometimes, greedy or backtracking algorithms help.

---

### 8. **Inclusion-Exclusion Principle**
- For coverings with overlaps or forbidden positions, use inclusion-exclusion to count valid configurations.
- Carefully define the sets to be included or excluded (e.g., placements violating constraints).
- Consider overcounting: subtract cases where two or more forbidden overlaps occur, add back cases where three overlap, etc.
- Inclusion-exclusion is especially useful when direct counting is hard due to complex restrictions.
- Drawing Venn diagrams or working through small examples can clarify the principle.

---

**Tip:**  
Start by solving small cases by hand to spot patterns, then generalize.

If you have a specific problem, share it for a tailored approach!



Problems set:
IMO 2025.6 = solution
IMO 2022.3


### Classic IMO Problems on Coverings and Tilings

- **IMO 1987 Problem 1**
- **IMO 1993 Problem 2**
- **IMO 1994 Problem 2**
- **IMO 2000 Problem 2**
- **IMO 2001 Problem 5**
- **IMO 2004 Problem 2**
- **IMO 2011 Problem 2**
- **IMO 2016 Problem 2**
- **IMO 2018 Problem 2**

### Suggested Textbooks and References

- **"Principles and Techniques in Combinatorics" by Chen Chuan-Chong and Koh Khee-Meng**  
    - See Chapter 7 (Tilings and Coverings), pp. 181–200.

- **"A Path to Combinatorics for Undergraduates" by Titu Andreescu and Zuming Feng**  
    - See Section 5.3 (Tiling Problems), pp. 142–148.

- **"Combinatorics: A Problem Oriented Approach" by Daniel A. Marcus**  
    - See Section 8.2 (Tiling Rectangles), pp. 179–183.

- **"Proofs from THE BOOK" by Martin Aigner and Günter M. Ziegler**  
    - See Chapter 9 (Domino Tilings), pp. 73–80.

- **"The Art and Craft of Problem Solving" by Paul Zeitz**  
    - See Section 11.3 (Tiling), pp. 312–318.

- **"Enumerative Combinatorics, Volume 1" by Richard P. Stanley**  
    - See Section 1.2 (Tilings), pp. 14–19.

- **"Combinatorial Problems and Exercises" by László Lovász**  
    - See Problems 6.1.1–6.1.10, pp. 184–188.

- **"Mathematical Olympiad Challenges" by Titu Andreescu and Razvan Gelca**  
    - See Section 6.2 (Coverings and Tilings), pp. 181–190.
Literatura