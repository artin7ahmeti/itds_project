# 📊 Introduction to Data Science Project

This repository contains the implementation of a data science project developed during the "Introduction to Data Science" course. The project is divided into three main exercises, each demonstrating the application of regression techniques to different types of data: analytical functions, synthetic multivariate data, and historical time series data.

---

## 📁 Project Structure

1. **Univariate Regression on Analytical Functions**
2. **Multivariate Regression on Synthetic Data**
3. **Temperature Series Forecasting**

---

## 1️⃣ Univariate Regression on Analytical Functions

In this section:
- Three analytical functions \\( f_1(x), f_2(x), f_3(x) \\) were defined.
- Regression models (Linear, Ridge, SVR, Random Forest, MLP) were tested.
- Feature engineering was introduced to improve predictions by adding polynomial and trigonometric features.
- Gaussian noise was injected to test robustness.

### Techniques Used:
- `LinearRegression`, `Ridge`, `SVR`, `RandomForestRegressor`, `MLPRegressor`
- Feature Engineering: \\( x^2, \\sin(x), \\cos(x), x^3, x\\sin(x) \\)
- Evaluation Metrics: `R²`, `Mean Squared Error`

---

## 2️⃣ Multivariate Regression on Synthetic Data

In this section:
- A synthetic dataset was generated using `make_regression` from `sklearn.datasets`.
- The model’s ability to handle multivariate data was tested.
- Scenarios with noise and non-informative features were introduced to evaluate robustness and feature interpretability.

### Techniques Used:
- Synthetic data with varying `n_features`, `n_informative`, and `noise`
- `LinearRegression` coefficients were analyzed to identify the impact of non-informative features.

---

## 3️⃣ Temperature Series Forecasting

In this section:
- Real weather data from WWII was used (source: Kaggle - https://www.kaggle.com/datasets/smid80/weatherww2).
- Mean temperatures from weather station `22508` (Honolulu, Hawai) were extracted and converted into a supervised dataset using rolling windows.
- A time-based train/test split was applied (Train: 1940–1944, Test: 1945).
- Forecasting models were trained and evaluated on one-day ahead predictions.
- Preprocessing strategies and hyperparameters were varied to evaluate model performance sensitivity.

### Techniques Used:
- Time series preprocessing with rolling windows
- LinearRegression, Ridge, RandomForestRegressor
- Evaluation with r2_score, mean_squared_error
- Visualization of predicted vs actual values
- Time-aware validation via `TimeSeriesSplit`

---

## 📦 Requirements

To run this project, install the following dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn
```
---

Link to this github repository: https://github.com/artin7ahmeti/itds_project
