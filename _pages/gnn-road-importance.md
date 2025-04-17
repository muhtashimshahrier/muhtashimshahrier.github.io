---
layout: single
title: "Road Segment Importance Prediction with GNNs"
permalink: /gnn-road-importance/
author_profile: true
---

## Road Segment Importance Prediction with GNNs

This project uses Graph Convolutional Networks (GCN) to classify road segments in **Dhaka** based on their relative importance, using real-world road data from OpenStreetMap. It combines graph feature engineering, multi-class labeling, and deep learning with PyTorch Geometric to explore scalable and interpretable models for transport networks.

---

### Project Goal

To classify whether a road segment is low, medium, or highly important based on graph structure and connectivity — without using traffic volume or speed data. This enables insight generation in data-sparse cities like Dhaka.

---

## Key Steps
The full drivable road network was extracted using **OSMnx**, then process it into a PyTorch Geometric graph and train both **MLP** and **GCN** models:

- **Feature Engineering**: Compute edge `length` and `betweenness centrality`.
- **Edge Labeling**: Assign multi-class labels based on OpenStreetMap `highway` tags.
- **Graph Conversion**: Convert to PyTorch Geometric format (`edge_index`, `edge_attr`, `edge_labels`).
- **Model Training**:
  - MLP (vanilla and class-weighted) trained on edge features only.
  - GCN model (`GCNConv`) trained to leverage graph structure for better generalization.

The pipeline was tested on both:
- A small subgraph of Dhanmondi (~2k edges), for rapid prototyping with MLP only.
- The full Dhaka network (~250k edges, 100k nodes), for city-scale GCN training.

---

## Note

This project was a hands-on attempt to understand how Graph Neural Networks (GNNs) can be applied to real-world transportation networks instead of using standard neural networks. I wanted to see if GNNs could pick up meaningful patterns from just the structure of the road graph — without any traffic flow or sensor data. Dhaka was used as a test case to explore how well this approach works in dense, data-sparse urban settings.


---

### 🔗 GitHub Repository

[muhtashimshahrier/GNN-road-importance](https://github.com/muhtashimshahrier/GNN-road-importance-)
