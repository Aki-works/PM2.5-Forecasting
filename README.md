# Multivariate Air Quality Forecasting Using Deep Learning Models 🌫️

> 📝 This repository contains the code, data preprocessing, model training scripts, evaluation metrics, and visualizations for my 'Essentials of AI and Machine Learning' course project during my B.Tech. in NIT, Calicut :  
> **"Multivariate Air Quality Forecasting Using Deep Learning Models: A Case Study on Delhi Pollution"**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) 

---

## 📌 Overview

Air pollution poses severe health, environmental, and economic challenges in urban centers like Delhi. This project applies a **multivariate LSTM-based deep learning approach** to forecast PM2.5 levels using historical pollutant concentrations and meteorological variables. By accurately predicting future pollution levels, this work aims to support smarter urban management and early warning systems.

---

## 🚀 Project Highlights

- **Problem**: Forecast PM2.5 pollution levels in Delhi using multivariate time series data.
- **Approach**: Multivariate LSTM model with lag and moving average features to capture temporal dependencies.
- **Data**: Kaggle Delhi Air Quality dataset (2015–2020)
- **Results**:  
  - MAE: 8.92 µg/m³  
  - RMSE: 14.14 µg/m³  
  - R² Score: 0.9746
- **Key Takeaway**: The model explained over 97% of the variance in PM2.5 concentrations, demonstrating strong predictive performance.

---

## 🗂️ Dataset

- **Source**: [Air Quality Data in India (Kaggle)](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
- **Features Used**: PM2.5, PM10, NO₂, CO, O₃, along with weather parameters
- **Frequency**: Hourly data

---

## 🛠️ Tech Stack

- Python (Pandas, NumPy, Matplotlib, scikit-learn)
- TensorFlow / Keras
- Jupyter Notebook
- Git / GitHub

---

## 📊 Methodology

1. **Data Preprocessing**
   - Missing value imputation with interpolation + forward/backward fill
   - Resampling to hourly frequency
   - Normalization with MinMaxScaler
   - Lag features and moving averages

2. **Model Building**
   - Two-layer LSTM with 64 and 32 hidden units
   - Dropout layers for regularization
   - Early stopping and dynamic learning rate
   - Dense output for PM2.5 prediction

3. **Evaluation**
   - MAE, RMSE, and R² as primary metrics
   - Visualization of predicted vs actual time series

---

## 📈 Results

| Metric | Value |
|--------|-------|
| **MAE** | 8.92 µg/m³ |
| **RMSE** | 14.14 µg/m³ |
| **R²** | 0.9746 |

<img width="1188" height="490" alt="image" src="https://github.com/user-attachments/assets/e7651eae-819e-4b36-ab69-521750fe6312" />

The LSTM model generalized well to unseen data and captured the key pollution patterns effectively.

