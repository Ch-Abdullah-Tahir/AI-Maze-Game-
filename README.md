# 🎮 Neon Maze Runner

A GUI-based maze adventure game built with Python and Tkinter that combines maze generation, AI decision-making, pathfinding, and constraint-based coin placement.

Players must navigate through a dynamically generated maze, collect coins, avoid a pursuing monster, and escape through a portal before the AI opponent reaches the exit.

---

## 🚀 Features

### 🧩 Dynamic Maze Generation

The maze is generated at runtime using **Prim's Algorithm**, ensuring a unique and fully connected maze in every game session.

### 🤖 Intelligent AI Opponent

An AI player competes against the human player using **Minimax with Alpha-Beta Pruning**. The AI analyzes future game states and chooses moves that maximize its chances of collecting coins.

### 👾 Monster Pathfinding

A monster hunts the leading player using the **A* (A-Star) Search Algorithm**, allowing it to find efficient paths through the maze.

### 🪙 Smart Coin Placement

Coins are placed using a **Constraint Satisfaction approach (CSP-inspired)** to maintain minimum distance between coins and avoid clustering.

### 🎨 Modern GUI

Built using Tkinter with:

* Neon-themed visuals
* Animated character sprites
* Portal effects
* Real-time score tracking
* Dynamic game state updates

---

## 🧠 Algorithms Used

| Component          | Algorithm                                       |
| ------------------ | ----------------------------------------------- |
| Maze Generation    | Prim's Algorithm                                |
| AI Decision Making | Minimax with Alpha-Beta Pruning                 |
| Monster Navigation | A* Search Algorithm                             |
| Coin Placement     | Constraint Satisfaction Strategy (CSP-inspired) |

---

## 🎯 Game Rules

* The player starts in the top-left corner.
* The AI starts in the top-right corner.
* The monster starts in the bottom-left corner.
* The exit portal is located in the bottom-right corner.
* Coins increase the player's score when collected.
* The portal remains locked for the first 15 turns.
* The monster gradually becomes more active:

  * Turns 0–4: Sleeping
  * Turns 5–9: Moves every alternate turn
  * Turn 10+: Moves every turn
* The game ends when:

  * The player reaches the exit after it unlocks.
  * The AI reaches the exit first.
  * The monster catches the player.

---

## 🕹 Controls

| Key   | Action       |
| ----- | ------------ |
| ↑     | Move Up      |
| ↓     | Move Down    |
| ←     | Move Left    |
| →     | Move Right   |
| Space | Restart Game |

---

## 📂 Project Structure

```text
├── main.py          # GUI and game rendering
├── logic.py         # Maze generation, AI, A*, Minimax
├── player.png
├── robot.png
├── monster.png
├── portal.png
└── README.md
```

---

## 🛠 Technologies Used

* Python 3
* Tkinter
* Pillow (PIL)
* Heapq
* Object-Oriented Programming

---

## 📚 Concepts Demonstrated

* Artificial Intelligence
* Game Development
* Search Algorithms
* Pathfinding
* Adversarial Search
* Constraint Satisfaction
* Event-Driven Programming
* Data Structures and Algorithms
* Object-Oriented Design

---

## ▶️ How to Run

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Install dependencies.

```bash
pip install pillow
```

3. Run the game.

```bash
python main.py
```

---

## 📖 Educational Purpose

This project was developed as an academic demonstration of how multiple AI techniques can be integrated into an interactive game environment. It showcases the practical application of maze generation, adversarial search, pathfinding, and constraint satisfaction techniques in a single project.

---

## 👨‍💻 Author

Developed as part of an Artificial Intelligence and Game Development learning project using Python.
