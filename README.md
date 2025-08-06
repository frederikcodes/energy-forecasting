# Energy Consumption Forecasting 🏠⚡

This repository contains a comprehensive time series forecasting project on household electricity consumption (Global Active Power) using SARIMA, Prophet, and LSTM (PyTorch).

---

## 📁 Project Structure

- `notebook.ipynb` – Jupyter notebook with full analysis: data cleaning, EDA, modeling, forecasting, and evaluation.
- `README.md` – This file.
- *(Data not included for size/license reasons.)*

---

## 📊 Data Source

The dataset originates from the UCI Machine Learning Repository and is hosted on Kaggle:  
**"Household Electric Power Consumption"** — electric power consumption measurements in one household at one-minute intervals over nearly four years (December 2006–November 2010) :contentReference[oaicite:1]{index=1}.

---

## 🧰 Tools & Libraries Used

- `pandas`, `numpy`, `matplotlib`, `seaborn` – for data manipulation and visualization  
- `statsmodels` – to implement SARIMA models  
- `fbprophet` (Prophet) – for automated trend and seasonality forecasting  
- `scikit-learn` – for scaling and error metrics (RMSE, MAE)  
- `torch` (PyTorch) – for building and training the LSTM neural network  


---

## 🛠️ What’s in the Notebook?

1. **Data Loading & Cleaning** – parsing date/time, handling missing values, resampling.
2. **Exploratory Data Analysis (EDA)** – global daily plots, autocorrelation, seasonality insights.
3. **Forecasting Methods**:
   - **SARIMA** (seasonal ARIMA) with parameter grid-search using AIC,
   - **Prophet** (robust to trend shifts and missing data),
   - **LSTM** (deep learning-based sequence modeling using PyTorch).
4. **Model Evaluation** – Forecast vs. actual plots; performance compared using RMSE and MAE at hourly and daily aggregation.
5. **Conclusion & Lessons Learned** – interpretation, strengths/weaknesses, and suggestions for future extension (e.g. external features).

---

## ✅ Usage Instructions

To replicate this project:
1. Download the dataset from [Kaggle: Household Power Consumption Dataset](https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set).
2. Unzip and place `household_power_consumption.txt` in the repository root directory.
3. Open and run Time_Series.ipynb in Jupyter.

## 📌 Key Learnings

- Forecasting on real-world time series requires **careful handling of missing data and seasonality**.
- **Prophet consistently outperformed SARIMA and LSTM** in both accuracy and forecasting realism.
- **LSTM demonstrated potential** but required more data preprocessing and tuning.
- **Visual and metric-based model comparison** (e.g., RMSE, MAE, daily vs. hourly) is essential to assess real-world usability.

---

This project demonstrates hands-on capability in time series forecasting methods, thoughtful data analysis, and clear evaluation—**ideal for applications in energy analytics, demand planning, or predictive modeling roles.**

---

**License:** MIT License

Enjoy exploring and feel free to reach out with any questions or feedback!
