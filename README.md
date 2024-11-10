# An ARIMA-LSTM model for predicting volatile agricultural price series with random forest technique

This repository contains predictive models for crop prices, focusing on **Arhar**, **Gram**, and **Moong**. 
The models use a combination of time-series analysis and machine learning techniques, including ARIMA, SARIMA, 
and ARIMA-LSTM hybrid models, to forecast future prices based on historical data from **01/2014 to 09/2024**.

## Files

### 1. [Arhar Prediction Model](./Arhar_prediction_model.ipynb)
- **Description**: This notebook provides a comprehensive analysis and prediction of Arhar crop prices using ARIMA, SARIMA, and ARIMA-LSTM models.
- **Key Steps**:
  - Exploratory Data Analysis (EDA) including stationarity tests (Phillips-Perron and ADF).
  - Seasonal decomposition to identify trends and seasonality.
  - Model tuning and selection using Auto-ARIMA to identify the best ARIMA parameters.
  - Hybrid modeling using ARIMA-LSTM to capture both linear and non-linear patterns.
  - Forecast evaluation using RMSE and other metrics, with residual analysis for validation.

### 2. [Gram Prediction Model](./Gram_prediction_model.ipynb)
- **Description**: This notebook focuses on predicting Gram crop prices.
- **Key Steps**:
  - Performs EDA and preprocessing, including stationarity testing.
  - Seasonal decomposition to isolate seasonal trends.
  - Model selection using Auto-ARIMA, with SARIMA and ARIMA-LSTM models.
  - Forecasting and model diagnostics, including residual analysis to validate assumptions.
  - Prediction and error estimation with RMSE for validation.

### 3. [Moong Prediction Model](./Moong_prediction_model.ipynb)
- **Description**: Predicts Moong crop prices using ARIMA, SARIMA, and ARIMA-LSTM models.
- **Key Steps**:
  - Data exploration and visualization of trends and seasonality.
  - Auto-ARIMA to determine optimal ARIMA model order.
  - Fitting ARIMA, SARIMA, and ARIMA-LSTM models.
  - Visualization of predictions, residual distribution, and error metrics for model evaluation.

### 4. [Price Dataset](./Price_dataset.csv)
- **Description**: Contains monthly price data for Gram, Moong, and Arhar crops from **01/2014 to 09/2024**.
- **Columns**:
  - `Date`: Monthly timestamp (YYYY-MM format).
  - `Gram`: Price data for Gram.
  - `Moong`: Price data for Moong.
  - `Arhar`: Price data for Arhar.

## Dependencies
- Python packages required:
  - `pandas`, `numpy`: For data handling and processing.
  - `matplotlib`: For data visualization.
  - `statsmodels`: For statistical and time-series modeling (ARIMA, SARIMA).
  - `arch`: For GARCH modeling on residuals.
  - `pmdarima`: For automated ARIMA model selection.
  - `tensorflow` or `keras`: For LSTM modeling in ARIMA-LSTM hybrid model.

Install dependencies using:
```bash
pip install pandas numpy matplotlib statsmodels arch pmdarima tensorflow





