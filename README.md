# Flood Prediction with Spatio-Temporal Graph Neural Networks

**Imperial College London – AI for Tackling Climate Change (2025/26)**

**Felicia Preuss-Neudorf, Maxime Brennion, Tim-Wei Schüler**

---

## Overview

This project develops and evaluates spatio-temporal Graph Neural Network (GNN) models for urban flood prediction. Given a sequence of historical water levels and rainfall, the models predict water level changes across all nodes in a 1D pipe network and a 2D surface mesh simultaneously.

## Repository Structure

### `training/`

**Temporal models:**

| Notebook | Description |
|---|---|
| `temporal_gru_model1.ipynb` | GAT + GRU, City 1 |
| `temporal_gru_model2.ipynb` | GAT + GRU, City 2 |
| `temporal_lstm_model1.ipynb` | GAT + LSTM, City 1 |
| `temporal_lstm_model2.ipynb` | GAT + LSTM, City 2 |
| `temporal_tcn_model1.ipynb` | GAT + TCN, City 1 |
| `temporal_tcn_model2.ipynb` | GAT + TCN, City 2 |

**Spatial models:**

| Notebook | Description |
|---|---|
| `spatial_gcn_model1.ipynb` | GCN + GRU, City 1 |
| `spatial_gcn_model2.ipynb` | GCN + GRU, City 2 |
| `spatial_sage_model1.ipynb` | SAGE + GRU, City 1 |
| `spatial_sage_model2.ipynb` | SAGE + GRU, City 2 |

### `eval/`

**Temporal models:**

| Notebook | Description |
|---|---|
| `srmse-temp-gru-m1.ipynb` | SRMSE evaluation, GAT+GRU, City 1 |
| `srmse-temp-gru-m2.ipynb` | SRMSE evaluation, GAT+GRU, City 2 |
| `srmse-temp-lstm-m1.ipynb` | SRMSE evaluation, GAT+LSTM, City 1 |
| `srmse-temp-lstm-m2.ipynb` | SRMSE evaluation, GAT+LSTM, City 2 |
| `temp-srmse-tcn-m1.ipynb` | SRMSE evaluation, GAT+TCN, City 1 |
| `temp-srmse-tcn-m2.ipynb` | SRMSE evaluation, GAT+TCN, City 2 |

**Spatial models:**

| Notebook | Description |
|---|---|
| `srmse-spatial-gcn-m1.ipynb` | SRMSE evaluation, GCN+GRU, City 1 |
| `srmse-spatial-gcn-m2.ipynb` | SRMSE evaluation, GCN+GRU, City 2 |
| `srmse-spatial-sage-m1.ipynb` | SRMSE evaluation, SAGE+GRU, City 1 |
| `srmse-spatial-sage-m2.ipynb` | SRMSE evaluation, SAGE+GRU, City 2 |

### Root files

| File | Description |
|---|---|
| `01_Model_Comparison.xlsx` | Aggregated SRMSE results across all models |
| `descriptive_data_analysis.ipynb` | Dataset statistics and rainfall analysis |
| `final-presentation-submission.pptx` | Final presentation slides |
| `README.md` | This file |

> **Note:** All SRMSE evaluation notebooks are built so that they match the evaluation code and procedure in the Kaggle Challenge. Link to Kaggle competition: https://www.kaggle.com/competitions/urban-flood-modelling/overview. Training notebooks are built so that they are comparable to each other in terms of evaluation.
