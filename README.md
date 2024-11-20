# Ship Route Optimization

This project implements a dynamic programming algorithm to calculate the optimal route for a ship navigating through a grid-like environment with obstacles. The ship must minimize its travel cost while avoiding obstacles and adhering to constraints such as course changes and collision avoidance.

---

## Features
- **Dynamic Programming Approach**: Efficiently computes the optimal route.
- **Obstacle Avoidance**: Handles moving obstacles with specified velocities and safe distances.
- **Waypoint Discretization**: Creates a grid of possible waypoints based on user-defined parameters.
- **Cost Function**: Considers distance and angle between waypoints to calculate optimal paths.

---

## How It Works
The program discretizes the ship's possible waypoints and calculates costs using:
1. **Distance between waypoints**: Determines the physical travel cost.
2. **Angle changes**: Penalizes sharp turns, ensuring smooth routes.

The dynamic programming algorithm evaluates the feasibility of transitions between waypoints and identifies the optimal predecessor for each state to minimize total cost.

---

## Prerequisites
- Python 3.7+
- `numpy` library

Install numpy if not already installed:
```bash
pip install numpy
