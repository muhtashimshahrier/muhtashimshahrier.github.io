---
layout: single
title: "Four-Step Travel Demand Model (Synthetic City)"
permalink: /four-step-model/
author_profile: true
---

This project implements the classical four-step travel demand model — **trip generation, trip distribution, mode choice, and traffic assignment** — from scratch for a synthetic 5-zone city. Each step was programmed and executed using Python, with full control over inputs and logic.

The goal was to develop a custom-coded version of the four-step model as a hands-on learning exercise in demand modeling and transport systems analysis.

---

## 🔄 Model Steps

- **Trip Generation**: Synthetic population, household, and employment data were used to generate trips from each zone.
- **Trip Distribution**: Gravity model used to estimate OD matrix based on impedance (travel cost).
- **Mode Choice**: Simplified multinomial logit model to allocate trips to private or public modes.
- **Traffic Assignment**: Deterministic shortest-path assignment using Dijkstra’s algorithm.

---

## 🛠 Tools Used
- Python
- NumPy, pandas
- NetworkX (for graph-based assignment)
- Matplotlib (for basic plotting)

---

## 📊 Outputs
- Zone-level O-D matrices for both Auto and Transit
- Network graph with edge labels for travel time and capacity
- All-or-nothing assigned flows visualized using edge width

---

[GitHub Repository](https://github.com/muhtashimshahrier/Custom-Four-Step-Demand-Model-From-Scratch-)

