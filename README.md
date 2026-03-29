# GNN Thermal Hotspot Prediction

Modeled chip thermal data as graph-structured meshes and trained a Graph Neural Network (GNN) to predict thermal hotspot locations.

## Overview
- Simulated 2D chip mesh data with node features: position, thermal conductivity, power density
- Built a 3-layer GCN using PyTorch Geometric
- Compared GNN performance against an MLP baseline

## Results
| Model | Accuracy | F1 (Hotspot) |
|-------|----------|--------------|
| GNN   | XX%      | 0.XX         |
| MLP   | XX%      | 0.XX         |

## Tech Stack
Python, PyTorch, PyTorch Geometric, scikit-learn, Matplotlib

## How to Run
Open the notebook in Google Colab and run all cells top to bottom.
