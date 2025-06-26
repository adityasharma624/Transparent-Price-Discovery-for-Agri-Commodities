# Transparent Price Discovery for Agri-Commodities

This project addresses the issue of market price volatility in agricultural commodities by leveraging time series forecasting and machine learning. By predicting daily prices for key vegetables—potato, onion, and tomato—we aim to reduce farmer exploitation, inform policy decisions, and enhance market efficiency.

---

## 📌 Problem Statement

Agricultural markets in India suffer from unpredictable price fluctuations, which hurt both farmers and consumers. These fluctuations complicate interventions like the Minimum Support Price (MSP) and Price Stabilization Fund (PSF). This project aims to:

- Forecast short-term price movements
- Provide data-backed insights to support market transparency
- Help farmers make informed decisions and reduce dependence on intermediaries

---

## 🧠 Techniques & Tools Used

- **Languages & Libraries**: Python, pandas, numpy  
- **Machine Learning**: XGBoost, SARIMAX, LSTM (Keras/TensorFlow)  
- **Visualization**: matplotlib, seaborn  
- **Development Environment**: Jupyter Notebook  
- **Data Source**: Agmarknet (arrival and price data)

---

## 🔍 Approach

1. **Data Collection**  
   Acquired historical daily prices and arrivals of potato, onion, and tomato from Agmarknet.

2. **Feature Engineering**  
   Applied lag-based features, rolling averages, exponential smoothing, and log transformations to highlight trends and seasonality.

3. **Exploratory Data Analysis (EDA)**  
   Visualized seasonal price patterns, supply spikes, and anomalies.

4. **Modeling**  
   Compared three forecasting models:
   - **SARIMAX**: Statistical time series model
   - **LSTM**: Deep learning sequence model
   - **XGBoost**: Tree-based regression model

5. **Evaluation**  
   Assessed models using:
   - R² Score
   - RMSE

---

## 📊 Results

- **XGBoost** achieved the highest accuracy with R² scores nearing **0.99**, showing strong predictive power.
- **LSTM** performed moderately well and set a realistic benchmark.
- **SARIMAX** underperformed, with negative R² scores on real-time data.
- Engineered features significantly improved temporal learning across models.

---

## 🚀 Future Work

- Integrate real-time market data via APIs (e.g., APMC)
- Deploy a web-based dashboard for farmers and policymakers
- Expand forecasting to more commodities and regions
- Incorporate rainfall, climate, and logistics data for enhanced prediction

---

## 📁 Project Structure
├── data/ # Raw and processed data
├── notebooks/ # Jupyter notebooks for EDA and modeling
├── results/ # Plots, metrics, and model outputs
├── README.md # Project documentation
