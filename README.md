# 🪙 Gold Price Prediction using Random Forest Regressor

This repository contains a Machine Learning project focused on predicting gold prices (GLD) using historical financial data. The model is built using the **Random Forest Regressor** and achieves high accuracy by analyzing several market indicators.

## 📊 Project Overview
Predicting the price of gold is a challenging task due to its dependence on various global economic factors. This project follows a structured Data Science workflow:
* **Data Cleaning:** Handling missing values and ensuring data integrity.
* **Exploratory Data Analysis (EDA):** Analyzing correlations between gold and other assets like Silver (SLV) and Oil (USO).
* **Model Development:** Implementing a Random Forest model with 100 estimators.
* **Hyperparameter Tuning:** Optimizing `max_depth` to 10 to prevent overfitting and improve generalization.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** - `Pandas` & `NumPy` (Data processing)
  - `Scikit-Learn` (Machine Learning)
  - `Seaborn` & `Matplotlib` (Visualization)

## 📁 Dataset
The dataset used in this project is sourced from **Kaggle**. It includes historical data for:
* **SPX:** S&P 500 Stock Index
* **GLD:** Gold Price (Target Variable)
* **USO:** United States Oil Fund
* **SLV:** Silver Price
* **EUR/USD:** Euro to US Dollar exchange rate

## 📈 Model Performance
After tuning the model to `max_depth=10`, the results demonstrated high reliability:

| Metric | Training Data | Test Data |
| :--- | :--- | :--- |
| **R² Score** | 0.998 | **0.991** |
| **MAE** | 0.672 | **1.320** |
| **RMSE** | 1.046 | **2.264** |

> **Key Insight:** By limiting the depth of the trees, we achieved a better balance between training and testing performance, ensuring the model performs well on unseen market data.
