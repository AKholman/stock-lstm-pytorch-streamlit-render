
# 🚀 AAPL Stock Price Forecasting App (PyTorch LSTM)

🔗 **Live App (Try it instantly):**  
https://akholman-deep-learning-stock-forecasting-app-app-uq0keh.streamlit.app/

---

## 📌 Overview

This repository contains the **deployment layer** of an end-to-end ML system for **next-day AAPL stock price prediction** using a **PyTorch LSTM model**.

The app provides an interactive dashboard built with **Streamlit**, where users can:
- Fetch latest AAPL market data
- Run inference using a trained LSTM model
- Visualize predicted vs actual prices

---

## 🧠 Model Overview

- Model: **LSTM (PyTorch)**
- Input: 60-day rolling window of OHLCV features
- Output: Next-day adjusted close price
- Feature scaling: MinMaxScaler
- Trained externally and loaded for inference only

---

## ⚙️ Tech Stack

- PyTorch (model inference)
- Streamlit (UI)
- Yahoo Finance (live data)
- Pandas / NumPy (data processing)
- Joblib (scalers)
- scikit-learn (preprocessing)

---

## 📂 Repository Structure

```
app.py                  → Streamlit inference app
best_lstm_model.pth    → Trained PyTorch model
scaler_X.joblib        → Feature scaler
scaler_y.joblib        → Target scaler
requirements.txt       → Dependencies
README.md              → Documentation
```

---

## 🚀 How It Works

1. Load latest AAPL data via Yahoo Finance
2. Apply saved MinMax scalers
3. Create 60-day sequences
4. Run PyTorch LSTM inference
5. Inverse transform predictions
6. Display results in Streamlit dashboard

---

## 📊 Features

- Real-time stock data fetching
- Next-day price prediction
- Interactive visualization
- Lightweight CPU deployment
- Fully reproducible inference pipeline

---

## ☁️ Deployment

- Hosted on **Streamlit Community Cloud**
- No backend server required
- Runs fully on CPU inference

---

## 🔗 Related Project

This is the **deployment layer** of a full ML system that includes:
- Model training (PyTorch + multiple ML models)
- Airflow orchestration
- MLflow experiment tracking
- Evidently monitoring

---

## 📌 Note

This app is for **educational and research purposes only**.  
Not financial advice.

---