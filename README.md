Description

This project implements a Pathfinding Visualizer using the A algorithm*.
It finds the shortest path between a start and end point in a grid while avoiding obstacles.

The A* algorithm combines Dijkstra's algorithm with a heuristic function, allowing faster and optimal pathfinding.

Features

Grid-based pathfinding with customizable start and end points

Handles obstacles and blocked cells

Implements A algorithm* from scratch

Prints the final path in the console, with the path marked using *

Easily extendable to GUI visualization using Pygame or Matplotlib

Grid Format

Represented as a 2D array:

0 → free cell (can walk through)
0 1 0 0 0
0 1 0 1 0
0 0 0 1 0
1 1 0 0 0
0 0 0 1 0
Usage

Clone the repository
git clone https://github.com/YOUR_USERNAME/AStar-Pathfinder.git
cd AStar-Pathfinder
Run the pathfinder script:

python astar_pathfinder.py


To use your own grid:

Add a grid file in sample_grids/ or modify the grid directly in astar_pathfinder.py

Update start and end coordinates accordingly

Output Example
Path found:
* 1 0 0 0
* 1 0 1 0
* * * 1 0
1 1 * * *
0 0 0 1 *


* marks the shortest path from start to end

How it Works

Heuristic Function: Uses Manhattan distance to estimate cost to the goal.

Priority Queue: Open set is implemented with a min-heap for efficient node selection.

Path Reconstruction: Tracks parent nodes to rebuild the path after reaching the goal.

Extensions (Optional)

Add GUI visualization using Pygame

Implement weighted grids

Animate the exploration process for better understanding

License

MIT License

1 → obstacle (cannot pass)

Example grid:
