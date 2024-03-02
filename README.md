
## Requirements

 - Python3
 - pygame

## How to run ?

 1. git clone https://github.com/iminoaru/Astar-mazeSolver.git
 2. cd Astar-mazeSolver
 3. install pygame if not already installed.
 4. run `python3 maze.py` in terminal.
 

## GUI controlling

- `space` runs the algorithm.
- orange represents start, blue represents goal, black represents obstacles.
- `C` to clear the map.
 

## About the Algorithm

 A* algorithm uses heuristic function `h(n)` and the exact distance between a node and the goal `g(n)`.

> f(n) = g(n) + h(n)

Formula used to calculate heuristic function is Manhattan Equation which is ideal for square grids. Taking D = 1 for simple calculations.

> h(n) = abs(node.x - goal.x) + abs(node.y - goal.y)

It maintains an openset which remains open until the corresponding `f(n)` to that node becomes minimum.

The value of the heuristic function h(n) is inversely proportional to accuracy (accuracy refers to the shortest path here) and directly proportional to speed of algorithm.


## Reference

This project was made with the help of Tim and [Heuristics by Stanford](https://theory.stanford.edu/~amitp/GameProgramming/Heuristics.html#)


