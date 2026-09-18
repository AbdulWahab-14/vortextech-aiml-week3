# vortextech-aiml-week3

# Vortex Tech Week 3 — Regression and Clustering on Real Data

This repository contains the Week 3 submission for the Vortex Tech AI/ML Internship track.

## Task Overview
This project implements supervised learning (Linear Regression) to predict house values and unsupervised learning (K-Means Clustering) to segment neighborhoods based on income and house prices using the California Housing Dataset.

---

## 1. Regression Task
- **Target Variable:** Median House Value (`MedHouseVal`)
- **Model:** Linear Regression (`scikit-learn`)
- **Train/Test Split:** 80% Training / 20% Testing (`random_state=42`)
- **Evaluation Metrics:**
  - **RMSE:** ~0.7455 (measures prediction error magnitude)
  - **R² Score:** ~0.5758 (explains ~57.6% of variance in house prices)

---

## 2. Clustering Task
- **Features Used:** `MedInc` (Median Income) and `MedHouseVal` (Median House Value)
- **Preprocessing:** Feature scaling using `StandardScaler`
- **Optimal Clusters (Elbow Method):** Evaluated $k=1$ to $10$. The "elbow point" occurred at **$k=3$**, indicating the point of diminishing returns for inertia reduction.
- **Cluster Interpretation:**
  - **Cluster 0:** Low Income / Low House Value
  - **Cluster 1:** Moderate Income / Moderate House Value
  - **Cluster 2:** High Income / High House Value

---

## How to Run
Open `Week3_Regression_Clustering.ipynb` in Google Colab or Jupyter Notebook and execute all cells sequentially.
