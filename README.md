


# FinSight: AI-Powered Real-Time Stock & Index Prediction & Strategy

A real-time stock and index prediction system using **Python, Machine Learning, and live market data**. This project predicts the next price of Nifty50 (or any stock/index) based on historical data and technical indicators.

---

## **Features**

- ✅ Predicts next-day stock/index price using a trained ML model.
- ✅ Real-time live prediction using Yahoo Finance data.
- ✅ Computes technical indicators such as:
  - SMA (Simple Moving Average) 20, 50, 200
  - RSI (Relative Strength Index)
  - MACD (Moving Average Convergence Divergence)
- ✅ Clean, modular Python code ready for integration with a frontend.
- ✅ Easy to extend to other stocks or indices.

---

## **How It Works**

1. **Data Collection:**
   - Historical stock/index data is fetched from **Yahoo Finance**.
   - Includes `Open, High, Low, Close, Volume, Adj Close`.

2. **Feature Engineering:**
   - Technical indicators are calculated from historical data:
     - **SMA20, SMA50, SMA200:** Smooth price trends.
     - **RSI:** Indicates overbought/oversold conditions.
     - **MACD & Signal Line:** Helps capture trend reversals.
   - Data is cleaned and converted to numeric format to ensure proper ML input.

3. **Model:**
   - A machine learning model (e.g., Random Forest or XGBoost) is trained on historical features.
   - The model learns the relationship between technical indicators and the next price.

4. **Prediction:**
   - The **latest row** of processed data is fed into the model.
   - Returns the predicted next price in real-time.

---

## **How to Run**

1. Clone the repository:

```bash
git clone https://github.com/bhukyasuresh24/stock-prediction.git
cd stock-prediction
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. To Run Live:
   ```bash
   python -m src.predict --symbol ^NSEI --live


## Folder Structure
- `data/raw/` → raw CSV files (historical data)
- `data/processed/` → cleaned & feature-engineered data
- `notebooks/` → Jupyter notebooks for EDA and modeling
- `src/` → Python scripts (data loading, feature engineering, models, strategy, backtesting)
- `models/` → saved ML/DL models
- `results/` → charts, performance reports
