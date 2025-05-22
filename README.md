

---

````markdown
# 🔥 Laser Labyrinth with Q-Learning

This is a Python implementation of a **Laser Maze Game** using **Q-Learning** for path planning and **Pygame** for visualization.

The agent starts from a given cell and learns to reach the goal while avoiding **moving laser beams** and **walls** in the grid.

---

## 📌 Features

- Reinforcement Learning using **Q-Learning**
- Moving **horizontal and vertical laser traps**
- Interactive visualization using **Pygame**
- Customizable grid, lasers, and training settings

---

## 🧠 How it Works

- The environment is a 2D grid (walls = `1`, open = `0`)
- Lasers sweep horizontally or vertically in a repeating pattern
- The agent learns the optimal path using Q-learning with a time-dependent state
- Reward system:
  - `-1` for each move
  - `-10` for hitting a laser
  - `+20` for reaching the goal

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/laser-maze-qlearning.git
cd laser-maze-qlearning
````

### 2. Install dependencies

Make sure you have Python 3.x installed. Then install the required libraries:

```bash
pip install numpy pygame
```

### 3. Run the code

```bash
python laser_maze.py
```

This will start training the agent and open a window for visualization after training.

---

## 🛠️ Customize Maze and Lasers

You can modify the grid, laser positions, start and goal cells:

```python
grid = [
    [0,0,0,0,0,0],
    [0,1,1,0,1,0],
    [0,1,0,0,1,0],
    [0,1,0,1,1,0],
    [0,0,0,0,0,0],
    [0,1,1,1,1,0],
]

lasers = [
    (2, 2, 'h', 6),  # horizontal laser
    (4, 4, 'v', 8),  # vertical laser
]

start = (0, 0)
goal = (5, 5)
```

---

## 📸 Preview

| Training (Console)       | Visualization (Pygame Window) |
| ------------------------ | ----------------------------- |
| Episode progress printed | Maze, agent, goal, lasers     |

---

## 📚 Concepts Used

* Q-learning with a time-modified state space
* Laser modeling using periodic phases
* Dynamic obstacle avoidance
* Gridworld navigation

---

## 📄 License

MIT License. Feel free to use and modify the project!

---

## ✨ Acknowledgment

Built with ❤️ using Python, NumPy, and Pygame.

