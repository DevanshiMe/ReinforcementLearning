

# Reinforcement Learning Explorations

This repository contains implementations of core **Reinforcement Learning (RL)** algorithms and their applications on custom environments built using **Gymnasium**.
Two environments are included — a **Normal GridWorld** and a more complex **WarehouseWorld**.
Both have accompanying visualizations to better understand agent behavior.


## Contents

### Algorithms Implemented

* **SARSA**
* **n-step SARSA**
* **Double Q-Learning**

### Environments

#### 1. Normal GridWorld

A 6×6 grid where the agent starts at `(0,0)` and explores to collect rewards.

* **Actions**: Up, Down, Right, Left, and Diagonal Down-Right (5 discrete actions).
* **Rewards**: Scattered across specific positions (5 → 100).
* **Goal**: Maximize total reward while navigating efficiently.

#### 2. WarehouseWorld

A more advanced environment inspired by warehouse navigation.

* **Item pickups** (reward = 25).
* **Drop-off location** (reward = 100).
* **Carrying state**: doubles the observation space (with/without item).
* **Obstacles (shelves)** block paths.
* **Actions**: 4 standard directions (no diagonal).
* **Goal**: Pick up items and deliver them to the drop-off point.

* Solved using **SARSA**, with visualizations.


## Key Takeaways

* Implemented **value-based RL algorithms** from scratch.
* Explored **custom Gymnasium environments** with both simple and complex tasks.
* Added **obstacles, carrying states, diagonal moves, and pickup/drop-off tasks** to test algorithm robustness.
* Visualizations provide insights beyond just numerical rewards.
