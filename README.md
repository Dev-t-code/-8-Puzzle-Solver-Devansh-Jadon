# 8 Puzzle Problem Solver (A* Search Algorithm)

## 📜 Description
This Python program solves the **8 Puzzle Problem** using the **A* Search Algorithm** with the **Manhattan Distance heuristic**. The **8-puzzle problem** consists of a 3x3 grid containing **8 tiles** and **one empty space** (represented by `0`). The objective of the puzzle is to **rearrange the tiles** from an **initial state** to a **goal state** by sliding the tiles up, down, left, or right.

The program takes the **initial state** and **goal state** from the user as input and then finds the optimal solution using the **A* Algorithm**.

---

## 💻 How to Run the Program

### **Step 1: Install Python**
Ensure you have Python 3.x installed on your computer. You can download it from [https://www.python.org/downloads/](https://www.python.org/downloads/).

### **Step 2: Run the Python Code**
1. **Open your terminal/command prompt**.
2. Navigate to the directory where the Python file is saved.
3. Run the command:
```bash
python 8_puzzle.py
```

---

## 📝 Input Format
The program expects the input as a **3x3 matrix** where:
- **Tiles are represented by numbers 1-8**.
- The empty space is represented by `0`.

### ✅ Example Input
**Initial State:**
```
1 2 3
4 5 6
7 0 8
```

**Goal State:**
```
1 2 3
4 5 6
7 8 0
```

You need to input these states manually during the program's execution.

---

## ✅ Output
The program will output the **step-by-step solution** to reach the goal state. It will display the intermediate states of the board, along with the minimum number of moves to solve the puzzle.

### Example Output
```
[1, 2, 3]
[4, 5, 6]
[7, 0, 8]

Move tile 8 down

[1, 2, 3]
[4, 5, 6]
[7, 8, 0]

Solution found in 1 step(s).
```

---

## 🚀 Algorithm Used
The program uses the **A* Search Algorithm (A-Star)** with the **Manhattan Distance** heuristic. Here's a brief explanation:

### **A* Search Algorithm**
- It uses both the **cost of the path (g(n))** and the **heuristic estimate (h(n))** to find the optimal solution.
- The heuristic function used in this code is the **Manhattan Distance**, which calculates the sum of the vertical and horizontal distances of each tile from its goal position.

### **Manhattan Distance Formula:**
```
h(n) = |x1 - x2| + |y1 - y2|
```
where:
- `x1, y1` = Current position of the tile.
- `x2, y2` = Target (goal) position of the tile.

---

## ✅ Constraints
1. The puzzle is only solvable if the **number of inversions** is even.
2. If the puzzle is unsolvable, the program will output:
```
No solution exists.
```

---

## 📂 Files
- **8_puzzle.py** - The main Python script that contains the logic for solving the puzzle.
- **README.md** - This file containing instructions to run the code.

---

## 💡 Future Improvements
1. ✅ Add a **Graphical User Interface (GUI)** using `Tkinter` or `Pygame`.
2. ✅ Allow the user to input the puzzle from a file.
3. ✅ Implement more heuristics like **Misplaced Tiles** or **Linear Conflict**.

---

## 🧑‍💻 Author
- **Created by:** [Your Name]
- **Date:** [Insert Date Here]

---

## 📜 License
This project is open-source and can be modified or distributed under the **MIT License**.

