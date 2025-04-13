---
layout: single
title: "Facility Location Optimization on a Synthetic Grid Using Monte Carlo Simulation"
permalink: /facility-location/
author_profile: true
---

## Facility Location Optimization on a Synthetic Grid Using Monte Carlo Simulation

This project simulates optimal facility placement on a synthetic 5×5 grid under travel time uncertainty. Each edge in the grid has a travel time drawn from a Gaussian distribution to reflect stochastic conditions. Monte Carlo simulation (1000 runs) is used to evaluate each facility’s performance based on travel time to random demand nodes.

The objective is to identify the most robust facility locations using average, 95th percentile, and worst-case travel times.

---

### Key Steps

- **Grid Generation**: Built a 5×5 grid network using NetworkX, with integer-labeled nodes.
- **Travel Time Modeling**: Assigned normally distributed travel times to each edge (mean and 20% standard deviation).
- **Demand Selection**: Randomly selected 5 demand nodes per simulation run; remaining nodes were used as facility candidates.
- **Monte Carlo Simulation**: Ran 1000 iterations, re-sampling edge travel times each time to simulate variability.
- **Facility Evaluation**: Ranked candidates based on average, 95th percentile, and worst-case travel time to all demand points.
- **Visualization**: Used matplotlib to plot network and highlight selected demand points.

---

### Repository

[🔗 View GitHub Repository](https://github.com/muhtashimshahrier/facility-location-montecarlo-grid)
