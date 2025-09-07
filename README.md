# Tic-Tac-Toe using Minimax Algorithm with Alpha-Beta Pruning

## Problem Statement
This project implements a **Tic-Tac-Toe game with Alpha-Beta Pruned Minimax Algorithm**. The rules are as follows:

- The board is a 3×3 grid.
- The player plays first as **X**.
- The computer plays second as **O**.
- The AI plays **optimally** and never loses.
- Alpha-Beta Pruning is used to **improve efficiency** by pruning unnecessary branches of the game tree.

---

## Time & Space Complexity

### Time Complexity
- **Without pruning (Minimax only):**
  - At most **9! game states**.
  - Minimax explores all possibilities:  
    **O(b^d)** where:  
    - *b* = branching factor (≤ 9)  
    - *d* = depth of game tree (≤ 9)  
  - Worst case: **O(9!) ≈ 362,880 states** (manageable).

- **With Alpha-Beta Pruning:**
  - Pruning reduces the number of states explored.
  - In the best case (perfect pruning):  
    **O(b^(d/2))** instead of **O(b^d)**.
  - This means the algorithm runs **much faster** while giving the **same optimal result**.

---

### Space Complexity
- **Recursion depth** = maximum depth of game tree = 9.  
- Hence, **O(d) = O(9)**.  
- Board state is stored as a vector globally.  
- Memory usage remains minimal.

---

## Use Cases
- **Classic demonstration** of the Minimax algorithm with Alpha-Beta Pruning.
- **Educational tool** for understanding:
  - Game theory
  - Recursion
  - Backtracking
  - Adversarial search
- Used in **AI game development** (tic-tac-toe, chess engines, connect four, etc.).
- Shows how pruning **improves efficiency** without changing the final outcome.

---

## Learning Outcomes
- Understand **Minimax algorithm** for adversarial games.
- Learn how **Alpha-Beta Pruning** reduces computational cost.
- Gain **hands-on coding experience** in:
  - Recursion
  - Backtracking
  - Optimal move decision-making
- Compare **heuristic search** vs **brute-force search**.
- Build intuition for **AI decision-making in games**.

---
