
### Problems set

# IMO 2024 Problem 5

## Problem Restatement

Turbo the snail plays a game on a \(2024 \times 2023\) board (2024 rows and 2023 columns).

- There are exactly 2022 hidden monsters placed on the board.
- Each row except the **first** and the **last** row contains **exactly one monster**.
- Each column contains **at most one monster**.
- Turbo starts any attempt on any cell in the **first row**.
- In each attempt, Turbo moves to adjacent cells sharing a side (up/down/left/right). He may revisit cells.
- If Turbo steps on a monster cell, the attempt ends immediately and Turbo returns to the first row to start a new attempt.
- If Turbo reaches any cell in the **last row**, the game ends successfully.
- Turbo remembers all monster cells discovered on previous attempts.

**Question:** Determine the minimum number \(n\) of attempts after which Turbo has a strategy that guarantees reaching the last row, regardless of how the monsters are placed.

---

## Math Area

This problem mainly belongs to:

- **Combinatorics and Graph Theory**
  - Pathfinding and connectivity on grids
  - Adversarial blocking / obstacle placement
- **Game Theory**
  - Strategies under partial/incomplete information
- **Algorithmic Combinatorics**
  - Search and elimination strategies

---

## Step-by-Step Solution Outline

1. **Model the board as a graph:**
   - Vertices represent cells.
   - Edges connect adjacent cells.
   - Monsters represent blocked vertices.

2. **Monster placement constraints:**
   - Exactly one monster in each row except first and last (2022 monsters).
   - Each column has at most one monster.

3. **Knowledge gained per attempt:**
   - Turbo can identify monsters by stepping on them.
   - After \(n\) attempts, Turbo can know at most \(n\) monster locations.

4. **Goal:**
   - Find a safe path from the first to the last row avoiding monsters.

5. **Lower bound on attempts:**
   - Since there are 2022 monsters, Turbo needs at least that many attempts to find them all if only one is discovered per attempt.

6. **Can Turbo find multiple monsters per attempt?**
   - Monsters are in different rows and columns, so one monster per row.
   - Turbo encounters at most one monster per attempt because stepping on a monster ends the attempt.

7. **Optimized strategy:**
   - Turbo can check columns systematically.
   - Since each column has at most one monster, checking columns one by one ensures discovery of all monsters or a safe path.

8. **Conclusion:**
   - Minimum number of attempts \(n = 2023\) (the number of columns).

---

## Summary

- Minimum attempts \(n = 2023\).
- Turbo’s strategy: explore columns to identify monsters and then find a safe path.

---

## Recommended Reading & Practice

### Core Topics

- Graph Theory: connectivity, paths, vertex blocking.
- Combinatorics: pigeonhole principle, counting.
- Game Theory: adversarial search and strategy.
- Grid pathfinding with obstacles.

### Books and Chapters

1. **"Introduction to Graph Theory" by Douglas B. West**  
   - Chapters on paths and connectivity.

2. **"A Path to Combinatorics for Undergraduates" by Titu Andreescu and Zuming Feng**  
   - Chapters on pigeonhole principle and combinatorial games.

3. **"Winning Ways for your Mathematical Plays" by Berlekamp, Conway, and Guy**  
   - Sections on combinational game theory.

4. **"Problem-Solving Strategies" by Arthur Engel**  
   - Chapters on combinatorics and graph theory.

### Practice Problems

- Grid pathfinding with obstacles.
- Combinatorial games on graphs.
- Adversarial search and elimination problems.

### Online Resources

- Art of Problem Solving (AoPS) forums: search for grid pathfinding and adversarial blocking.
- Brilliant.org courses on graph theory and combinatorics.
- IMO compendiums with similar problem types.

---

## Study Tips

- Master DFS, BFS algorithms.
- Understand pigeonhole principle applications.
- Practice worst-case scenario reasoning.
- Learn efficient exploration and information gathering strategies.

---

If you want, I can prepare a detailed worked example or simulate Turbo’s strategy on a smaller board.

