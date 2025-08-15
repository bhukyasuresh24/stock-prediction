# Stock Prediction & Performance Analysis

![Stock Prediction](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview
This project predicts stock/index prices using historical market data and machine learning models. It downloads live and historical stock data, processes features like moving averages, RSI, and MACD, and predicts the next value using a pre-trained model. It also generates performance reports comparing actual vs predicted prices.

This is a **full Python-based project** ready for real-time predictions, analysis, and performance reporting. It’s suitable for showcasing on your resume for campus interviews at top institutes like **IIT Indore**.

---

## 💡 Features
- Download **historical and live stock/index data** using Yahoo Finance API.
- Compute technical indicators:
  - SMA20, SMA50, SMA200 (Simple Moving Averages)
  - RSI (Relative Strength Index)
  - MACD & Signal Line
- Predict **next-day stock price** using a trained ML model.
- Generate **performance report** with metrics:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
  - MAPE (Mean Absolute Percentage Error)
- Visualize actual vs predicted prices with **Matplotlib charts**.
- Safe handling of single-row and live data to prevent errors.

---

## ⚡ How It Works
1. **Data Download**: Uses `yfinance` to download stock data.
2. **Feature Engineering**:
   - Computes technical indicators to form ML features.
   - Handles missing data and ensures numeric columns are safe.
3. **Model Prediction**:
   - Loads a pre-trained ML model (`nifty50_model.pkl`).
   - Uses last available row for live prediction or full historical data for performance analysis.
4. **Performance Report**:
   - Compares predicted vs actual prices.
   - Calculates metrics (MAE, RMSE, MAPE).
   - Generates plots for visualization.

---

## 🛠️ Setup & Installation

1. Clone the repository:

```bash
git clone https://github.com/bhukyasuresh24/stock-prediction.git
cd stock-prediction
---
## Install dependencies:

pip install -r requirements.txt
---
