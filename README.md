# Graph Convolutional Network Based Model for Megacity Real Estate Valuation

A real estate valuation framework designed for megacities, where property prices are influenced by spatial proximity and neighborhood relationships.

This project demonstrates how graph-based learning can be applied to real estate pricing, with a working prototype deployed using Django.

## Current Implementation (V1 - Deployed)

**Live Working Model:** Feature-based price prediction
- **Inputs:** No. of rooms, floors, sqft, BHK, location
- **Output:** Predicted property price
- **Stack:** Python, PyTorch, Scikit-learn, Django, MySQL
- **Model:** MLP baseline inspired by GCN spatial correlation concept

The model takes core property features and predicts price instantly.

## GCN Concept & Architecture (V2 - Research Phase)

Ideal GCN approach for megacity:
- **Nodes:** Individual properties / localities
- **Edges:** Spatial proximity (<2km), similar amenities, road connectivity
- **Node Features:** sqft, rooms, floors, distance to metro/school
- **Graph Conv Layer:** PyTorch Geometric - aggregates neighbor prices to predict target price
- **Why GCN?** Traditional regression treats houses as independent. GCN learns "price of house depends on neighborhood price" - critical for megacities like Hyderabad, Mumbai.

## Tech Stack
- Backend: Python, Django, PyTorch
- ML: PyTorch, Scikit-learn, Pandas, NumPy
- Database: MySQL
- Frontend: HTML, CSS (Django Templates)
- Graph Library (V2): PyTorch Geometric, NetworkX

## How to Run
