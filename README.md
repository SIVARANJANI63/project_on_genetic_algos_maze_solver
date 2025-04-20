# 🧠 Maze Solver using Genetic Algorithm

This project demonstrates how a Genetic Algorithm (GA) can be applied to solve a maze pathfinding problem. By simulating evolution through selection, crossover, and mutation, the algorithm learns to navigate from the start to the goal in a complex grid-based maze.

---

## 📌 Project Highlights

- 🧬 **Evolutionary Algorithm** with DEAP
- 🗺️ **Pathfinding in a Maze**
- 🖼️ **Visual Maze Path Plots**
- 📉 **Fitness based on Manhattan Distance**
- 🧪 Includes mutation, crossover, and selection

---

## 🧭 Maze Description

The maze is represented as a 2D grid:
- `0` = Walkable path
- `1` = Wall (blocked path)

The goal is to move from the **top-left corner** `(0, 0)` to the **bottom-right corner** `(14, 14)` avoiding walls.

---

## 🧮 Algorithm Logic

- **Individual Representation**: A list of directions (`['U', 'D', 'L', 'R']`)
- **Fitness Function**: Manhattan distance from the current position to the goal
- **Selection**: Tournament
- **Crossover**: Uniform crossover
- **Mutation**: Random directional changes

---

## 🔧 Dependencies

```bash
pip install matplotlib deap

```
## 🚀 How It Works

1. 🎲 **Random individuals (paths)** are created using directional moves: `'U'`, `'D'`, `'L'`, `'R'`.
2. 🧪 **Each individual is evaluated** by simulating its path in the maze.
3. 🏆 The algorithm **selects the fittest individuals**, applies **crossover** and **mutation** to create the next generation.
4. 🔁 This evolutionary process repeats for a fixed number of generations or until the path successfully reaches the goal.

---

## 📊 Visualization

At specific generations (e.g., Gen 2, 10, 50, 100, 500, Final), the best path found is visualized using `matplotlib`:

- ✅ **Start Point**: Green
- 🔵 **Path Traversed**: Blue
- 🔴 **Goal Point**: Red
- ⚫ **Walls**: Black
- ⚪ **Free Path**: White

Each path visualization shows how the algorithm learns and evolves better paths through generations!

---

## 📁 File Structure

```plaintext
maze_ga_solver.py      # Main script
README.md              # This file

```

🛠️ Improvements to Try
🧩 Add dynamic maze input from the user

➕ Introduce diagonal movements ('UL', 'UR', 'DL', 'DR')

🧠 Integrate with A* for hybrid optimization

💾 Save the best path and result to a file or export as image

🙌 Acknowledgements
🧬 DEAP – Distributed Evolutionary Algorithms in Python

📚 Inspiration from classic AI pathfinding problems and genetic programming techniques

📌 Author
Sivaranjani A
