# AI-Driven Waste Collection & Environmental Sampling Route Planner

An interactive web application and Python implementation for optimizing multi-stop vehicle routing, featuring graph-based search algorithms (A*, UCS, BFS), Traveling Salesperson Problem (TSP) solvers, real-time road blocking, and carbon emission estimation.

![Route Planner Preview](https://img.shields.io/badge/Status-Active-brightgreen)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![HTML5 Canvas](https://img.shields.io/badge/Frontend-HTML5%20%2F%20JavaScript-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 🚀 Features

- **Interactive Canvas Map:** Click to inspect junctions, toggle road closures, and visualize optimal vehicle routes in real time.
- **Advanced Graph Search Algorithms:**
  - **A\* Search:** Utilizes straight-line heuristic ($h$) for efficient node expansion.
  - **Uniform Cost Search (UCS):** Explores uniformly by path cost ($h=0$).
  - **Breadth-First Search (BFS):** Finds the minimum-hop route across intersections.
- **Multi-Stop Optimization (TSP):**
  - **Nearest-Neighbour Heuristic:** Fast greedy routing for visiting multiple bins/sampling sites.
  - **Brute-Force Optimal Tour:** Evaluates all permutations to guarantee the absolute shortest route.
- **Emergency Replanning:** Instantly recalculates alternative paths when specific roads or bridges are blocked.
- **Environmental Impact Modeling:** Optimizes routes based on estimated $\text{CO}_2$ emissions ($\text{kg CO}_2$) rather than raw distance alone.

---

## 🗂️ Project Structure

```text
├── index.html              # Interactive web application visualizer
├── route_planner.py        # Core Python 3 CLI implementation and algorithms
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Actions workflow for automatic GitHub Pages deployment
