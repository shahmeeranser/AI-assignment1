# Interactive Grid Planner

A visual pathfinding tool built with Python and Tkinter.

## Requirements

- Python 3.8+
- Tkinter (usually bundled with Python)

## Installation

**Windows / macOS**
```
python -m pip install --upgrade pip
python grid_planner.py
```

**Ubuntu / Debian**
```
sudo apt install python3-tk
python3 grid_planner.py
```

**Arch Linux**
```
sudo pacman -S tk
python grid_planner.py
```

## Usage

1. Place a **Start** node, an **End** node, and optionally draw **Obstacles**
2. Select an algorithm from the dropdown
3. Click **Run**

## Algorithms

| Algorithm | Description |
|---|---|
| BFS | Shortest path, unweighted |
| DFS | Explores deep before backtracking |
| IDS | Iterative deepening depth-first search |
| DLS | Depth-limited search — set max depth via spinner |
| Bidirectional | BFS from both ends simultaneously |
| UCS | Lowest-cost path — diagonals cost 2, cardinals cost 1 |
