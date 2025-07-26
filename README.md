# Jalayaan: Optimal Ship Routing Algorithm

## Overview

Jalayaan is a versatile and fast algorithm for optimal ship routing, with a specific focus on the Indian Ocean region. This project was developed for the Smart India Hackathon (SIH) 2024.

The primary goal is to determine the most efficient and safest route for a vessel by simultaneously considering multiple, often competing, objectives. The algorithm is designed to be adaptable for a range of ship types and evolving weather conditions.

***

## Key Features

* **Multi-Criteria Optimization:** The algorithm optimizes routes based on three core parameters:
    * **Fuel Consumption:** Minimizing fuel usage to reduce operational costs and environmental impact.
    * **Voyage Time:** Ensuring the fastest possible transit.
    * **Safety/Risk:** Evaluating environmental factors to avoid conditions that could endanger the vessel, cargo, and crew.
* **Indian Ocean Specific:** Tailored to address the unique maritime conditions and lack of specialized routing tools for the Indian Ocean.
* **Hybrid Algorithmic Approach:** Combines multiple powerful optimization techniques to find a robust solution.
* **Versatile & Adaptable:** Built with a scope to add more optimization parameters and handle various ship types and characteristics.

***

## Technical Approach

The core of this project is a hybrid algorithm that leverages the strengths of several well-established methods in pathfinding and optimization. The methodology is inspired by the work on multi-criteria ship routing by **Wei Zhao, et al.**

The algorithms employed include:
1.  **A\* Algorithm:** Used for initial pathfinding on a grid, efficiently finding a feasible route from the start to the destination.
2.  **Particle Swarm Optimization (PSO) & Genetic Algorithm (GA):** These metaheuristic algorithms are used to refine and optimize the initial path. They explore a wide range of possible route variations to find a set of non-dominated solutions (the Pareto front) that represent the best possible trade-offs between fuel, time, and safety.

***

## Data Source

**Note:** The current implementation utilizes a simulated dataset for the purpose of algorithm development, testing, and demonstration. For a real-world application, this module would be integrated with live data streams for surface winds, currents, and waves from official sources like the Indian National Centre for Ocean Information Services (INCOIS).

***

## How to Run

1.  **Prerequisites:** Ensure you have Python installed with the following libraries:
    * `numpy`
    * `matplotlib`

2.  **Execution:**
    * Open the `Ship_routing (1).ipynb` file in a Jupyter Notebook environment (like Jupyter Lab or Google Colab).
    * Execute the cells in sequence to run the simulation and visualize the optimal route.
