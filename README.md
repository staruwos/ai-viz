# AI-Viz

A 3D pathfinding playground and AI visualization tool for games, built with Three.js. 

## Overview

AI-Viz provides an interactive environment to visualize and compare pathfinding algorithms and simple game-AI behaviors. It parses a 3D grid where users can edit obstacles, define start/end nodes, and observe the search frontier and path reconstruction in real-time.

[Live Demo](https://julionico.online/systems/ai-viz/index.html)

## Features

* Pathfinding Algorithms: A* Search, Dijkstra, Breadth-First Search (BFS), and Greedy Best-First Search.
* Agent Behaviors: "Move to Goal", "Patrol" (continuous looping between nodes), and "Wander" (random valid node selection).
* Interactive Environment: Raycast-based map editing to toggle walls and update objectives on the fly.
* Zero Build Step: Pure client-side application using vanilla JavaScript and ES6 module imports.

## Local Deployment

Because the application relies on ES6 module imports (via an import map) for Three.js, the files must be served over an HTTP connection rather than accessed directly via the local `file://` protocol.

1. Clone the repository:
```bash
git clone https://github.com/staruwos/ai-viz.git
cd ai-viz
```

2. Start a local HTTP server. For example, using Python:
```bash
python3 -m http.server 8080
```

3. Access the application in your browser at `http://localhost:8080`.

## Technology Stack

* Frontend: HTML5, CSS3, Vanilla JavaScript
* Rendering: WebGL via Three.js
* Dependencies: Three.js and OrbitControls (loaded at runtime via CDN)

## License

MIT License. See LICENSE for more information.
