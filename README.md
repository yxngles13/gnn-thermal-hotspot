# GNN Thermal Hotspot Prediction

Modeled chip thermal data as graph-structured meshes and trained a 
GraphSAGE Graph Neural Network (GNN) to predict thermal hotspot locations.

## Overview
- Simulated a 300-node 2D chip mesh with realistic heat sources using 
  Gaussian thermal spread
- Connected nodes using k-nearest neighbor (k=6) graph construction
- Node features: spatial position, thermal conductivity, power density
- Trained on 80% of nodes, evaluated on unseen 20% test set

## Results
| Model | Accuracy | F1 (Hotspot) |
|-------|----------|--------------|
| GNN (GraphSAGE) | 85% | 0.76 |
| MLP Baseline | 95% | 0.91 |

## Key Takeaway
The MLP outperforms on simulated data because features alone are 
sufficient. GNNs are expected to outperform on real chip meshes where 
neighboring nodes thermally influence each other — exactly the use case 
at companies like Cadence.

## Visualization
<img width="653" height="528" alt="download" src="https://github.com/user-attachments/assets/355371dc-81d8-4d6c-9c02-4f10de44a0d4" />

## Tech Stack
Python, PyTorch, PyTorch Geometric, scikit-learn, Matplotlib, Google Colab

## How to Run
Open the notebook in Google Colab and run all cells top to bottom.
