## Path Finding Visualizer

This is a project for visualizing the shortest path from source to destination. The project also focuses on the different ways the algorithm can traverse nodes. Theoretically, the possible "moves" are endless. The current moves used in the application are based on chess moves (rook, bishop, and queen).

<h1>React.js Shortest-Path-Visualizer App</h1>
<br>
## find the website live [here](https://salmon-sea-03f0b461e.5.azurestaticapps.net)

## 💻 Tech Stack

- React
- Javascript
- HTML
- CSS
- Microsoft Azure

## Some well known Algorithms

DFS: a common traversing algorithm that prioritizes going as deep as possible until all possible nodes have been visited and discovered, before traversing other neighbor nodes.

BFS: another common traversing algorithm that prioritizes closest neighbors first, before exploring the depth.

Dijkstra's shortest path: A very famous algorithm, commonly used in modern day applications. The algorithm revolves around a priority queue, and updates the visited nodes with the lowest possible distance value. By the time the target node is reached, because of how priority queue works, it would have guaranteed the shortest path to reach that node. 

A*: A variation of Dijkstra's shortest path. A* updates the priority queue based on the shortest possible path from the start AND also a value called heuristic value. The heuristic value can be any value of "distance", depending on how the heuristic is calculated, the traversing of the the nodes may look different. Common heuristic values are the manhattan distance, euclidean distance, there are many more, this is what makes A* a really flexible algorithm. A* is capable of doing Dijkstra's algorithm smarter based on certain parameters. Common applications for this algorithm are used in how GPS routing works with traffic, tolls, physical distance, time traveled and many more. In this application we have chosen both the manhattan distance and euclidean distance as our primary heuristic value calculation (manhattan for rook mode, and euclidean for bishop/queen mode)

## Modes

**Rook**: Traversing direction that can only move vertically and horizontally. <br>
**Bishop**: Traversing direction that can only move diagonally, only diagonal nodes are ever explored, making it possible to cut through unsealed corners. Roughly half of the nodes in the grid will be unexplorable by this mode. <br>
**Queen**: Traversing direction that can move vertically, horizontally, and diagonally. This mode can cut through unsealed corners. Undoubtedly, this mode is the most efficient way to traverse through the grid.

## Running the application

clone the repo
```
    npx create-react-app my-app
    cd my-app
    npm start

```
then ```npm run```. You can then access the application on ```localhost:3000```.
## find the website live [here](https://salmon-sea-03f0b461e.5.azurestaticapps.net)
