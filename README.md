# Informed Search Visualizer

A Python-based grid pathfinding visualizer implementing informed search algorithms with dynamic obstacle support.

## Features

### Search Algorithms
- **Best-First Search** - Greedy search using heuristic distance
- **A* Search** - Optimal pathfinding with f(n) = g(n) + h(n)

### Heuristics
- Manhattan Distance
- Euclidean Distance

### Dynamic Mode
- Real-time obstacle spawning during agent transit
- Automatic path re-planning on collision
- Efficient re-computation from current position

### Grid Controls
- Place start, end, and obstacle cells
- Random maze generator with adjustable density
- Adjustable grid size (3-60 columns, 3-40 rows)
- Auto-scaling cell size for larger grids

## Requirements

```
Python 3.x
tkinter (usually included with Python)
```

## Usage

```bash
python grid_program.py
```

## Controls

### Modes (Left Panel)
- **Start** - Place start point
- **End** - Place end point  
- **Obstacle** - Draw obstacles
- **Erase** - Clear cells

### Actions (Right Panel)
- **Clear Grid** - Reset entire grid
- **Clear Obstacles** - Remove all obstacles
- **Apply Size** - Change grid dimensions
- **Generate Maze** - Create random maze
- **Run Search** - Execute selected algorithm
- **Stop** - Halt current simulation
- **Clear Path** - Remove search visualization

### Dynamic Mode
- Enable checkbox to activate obstacle spawning
- Adjust spawn probability (1-20%)
- Watch agent re-plan around new obstacles

### Mouse Controls
- **Left Click** - Place in current mode
- **Right Click** - Erase cell
- **Drag** - Paint obstacles or erase quickly

## Color Code

| Color | Meaning |
|-------|---------|
| Orange | Start point |
| Pink | End point |
| Dark Gray | Obstacle |
| Yellow | Cells in queue (frontier) |
| Blue | Visited/explored cells |
| Green | Final path |
| Purple | Agent position (dynamic mode) |
| Red | Dynamically spawned obstacle |

## Metrics

After successful pathfinding:
- **Nodes Visited** - Total expanded nodes
- **Path Cost** - Length of final path
- **Execution Time** - Computation time (ms)
- **Replans** - Re-calculations in dynamic mode
