---
layout: single
title: "Road Segment Importance Prediction with GNNs"
permalink: /gnn-road-importance/
author_profile: true
---

## Road Segment Importance Prediction with GNNs

This project uses Graph Neural Networks (GNNs) to classify road segments in **Dhaka** based on their relative importance, using real-world road data from OpenStreetMap. It combines graph feature engineering, multi-class labeling, and deep learning with PyTorch Geometric to explore scalable and interpretable models for transport networks.

---

### 🔍 Project Goal

To classify whether a road segment is low, medium, or highly important based on graph structure and connectivity — without using traffic volume or speed data. This enables insight generation in data-sparse cities like Dhaka.

---

### 🧩 Key Steps

- **Graph download**: Retrieved the full drivable road network of Dhaka using OSMnx.
- **Edge labeling**: Assigned each road segment to one of four importance classes based on OpenStreetMap `highway` tags.
- **Feature engineering**: Computed `length` and `betweenness centrality` as edge-level features.
- **Graph conversion**: Transformed the graph to PyTorch Geometric format for edge classification.
- **Model training**:
  - Trained a baseline MLP on a small Dhanmondi subgraph (~2k edges)
  - Scaled up to the full Dhaka network (~250k edges)
  - Used class-weighted loss to address real-world label imbalance

---

### 🧠 Why It Matters

This project showcases how GNNs can be applied to real-world transportation networks, even in data-sparse settings. It demonstrates skills in:
- Graph theory & spatial networks
- Real-world data cleaning & labeling
- PyTorch Geometric model development
- Handling class imbalance in urban data

---

### 🔗 GitHub Repository

[muhtashimshahrier/GNN-road-importance](https://github.com/muhtashimshahrier/GNN-road-importance-)
