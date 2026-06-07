# Agentic AI for EV Charging Tariff Optimization

## Overview

This project develops an Agentic AI framework for intelligent EV charging tariff optimization using operational charging network data. The objective is to improve revenue, reduce congestion, encourage off-peak charging, and support efficient charger utilization through data-driven pricing decisions.

The solution combines machine learning-based demand forecasting with dynamic pricing recommendations and continuous performance monitoring.

---

## Problem Statement

Traditional fixed EV charging tariffs fail to account for fluctuations in charging demand, congestion levels, and charger utilization.

This project addresses the challenge by building:

* Demand Prediction Agent
* Tariff Pricing Agent
* Monitoring & Learning Agent

that work together to optimize charging network performance.

---

## Datasets Used

### UrbanEV Dataset

Used for:

* Demand Prediction Agent
* Charger Utilization Analysis
* Congestion Estimation
* Off-Peak Uplift Analysis
* Waiting Time Reduction Proxy

### ACN Charging Dataset

Used for:

* Revenue Gain Evaluation
* Customer Response Analysis
* Pricing Efficiency Measurement

---

## Project Architecture

UrbanEV Dataset

↓

Demand Prediction Agent

↓

Predicted Utilization Rate

Expected Charging Load

Congestion Probability

↓

Tariff Pricing Agent

↓

Dynamic Tariff Recommendation

(₹14 Discount / ₹15 Standard / ₹18 Surge)

↓

Monitoring & Learning Agent

↓

Performance Evaluation

↓

Revenue Gain

Utilization Analysis

Waiting Time Reduction

Customer Response

Pricing Efficiency

---

## Methodology

### 1. Data Preprocessing

* Integrated multiple charging datasets into a unified analytical base
* Handled missing values using interpolation and forward-fill techniques
* Standardized timestamps and station-level information

### 2. Feature Engineering

Created operational and economic features including:

* Charger Utilization Rate
* Revenue per Session
* Occupancy Density
* Queue Length Proxy
* Congestion Categories
* Fast Charger Ratio
* Charging Station Mix
* Peak Congestion Score

### 3. Exploratory Data Analysis

Analyzed:

* Hourly charging behavior
* Peak vs Off-Peak demand
* Weekday vs Weekend trends
* Station utilization patterns
* Fleet vs Public charging signatures
* Congestion distribution

### 4. Demand Prediction Agent

A Random Forest Regressor was trained to forecast:

* Predicted Utilization Rate
* Expected Charging Load
* Congestion Probability

### 5. Tariff Pricing Agent

Generated dynamic pricing recommendations based on predicted demand:

| Utilization Condition | Tariff |
| --------------------- | ------ |
| Low Demand            | ₹14    |
| Normal Demand         | ₹15    |
| High Demand           | ₹18    |

### 6. Monitoring & Learning Agent

Evaluated pricing outcomes using:

* Revenue Gain %
* Charger Utilization Rate
* Off-Peak Uplift
* Waiting Time Reduction
* Customer Response Rate
* Pricing Efficiency Score

---

## Model Performance

### Demand Prediction Agent

| Metric   | Value  |
| -------- | ------ |
| MAE      | 0.0068 |
| RMSE     | 0.0144 |
| R² Score | 0.9933 |

---

## Business Results

| KPI                      | Result     |
| ------------------------ | ---------- |
| Revenue Gain             | +9.46%     |
| Off-Peak Uplift          | +20.0%     |
| Waiting Time Reduction   | +5.0%      |
| Customer Response Rate   | +0.23%     |
| Pricing Efficiency Score | ₹16.38/kWh |

---

## Assumptions

* Energy cost assumed at ₹7/kWh for economic calculations.
* Fleet charging behavior identified using a utilization-duration proxy.
* Queue length estimated through occupancy-based congestion indicators.
* Customer response measured using elasticity-based assumptions.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Repository Structure

```text
01_Data_Loading.ipynb
02_Data_Preprocessing.ipynb
03_Feature_Engineering.ipynb
04_EDA.ipynb
05_Demand_Prediction_Agent.ipynb
06_Tariff_Pricing_Agent.ipynb
07_Monitoring_Learning_Agent.ipynb
08_ACN_Metrics.ipynb
09_Final_KPIs.ipynb

Outputs/
Presentation/
README.md
```

---

## Key Takeaway

The proposed Agentic AI framework demonstrates how predictive analytics and adaptive pricing strategies can improve EV charging network performance by increasing revenue, encouraging off-peak charging, and supporting smarter operational decision-making.
