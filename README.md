# 🌍 Smart Energy Management System (EMS)

## Project Overview
Optimization of a multi-energy industrial site (Heat & Cooling) using Machine Learning and Mixed-Integer Linear Programming (MILP). The goal is to minimize operational costs while ensuring a **60% Renewable Energy (EnR) target** is met over the year using a dynamic pilot.

## 🚀 Key Features
1.  **Forecasting:** Machine Learning models to predict Heat and Cooling loads based on weather data.
2.  **Digital Twin:** Modeling of a complex fleet (Gas Boilers, Biomass, Heat Pumps, Chillers) with efficiency and coupling constraints.
3.  **Optimization Engine:** A MILP solver (`PuLP`) that optimizes energy dispatch hour-by-hour.
4.  **Dynamic Pilot:** A Rolling Horizon algorithm that adjusts the strategy week-by-week to enforce the yearly EnR target.

## 🛠️ Stack & Tools
* **Python 3.x**
* **Pandas / NumPy** for data manipulation.
* **PuLP** for Linear Programming optimization.
* **Plotly** for interactive visualization.

## 📦 How to run
1.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib pulp plotly openmeteo_requests requests_cache retry_requests tqdm pulp
    ```
2.  Run the notebook `Projet_V1.ipynb`.

## 📊 Results
* Achieved **60% Renewable Energy Rate** on the test year (2024) du to 2025 wasn't finished.
* Zero load shedding (100% demand coverage).
* Automatic management of seasonality (Biomass baseload vs Gas peak).
