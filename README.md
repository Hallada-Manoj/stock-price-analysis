# Stock Price Analysis and Forecasting

## Project Overview

This project explores historical stock market data using Python, focusing on Apple Inc. (AAPL). It includes exploratory data analysis, financial data visualization, outlier detection, and time-series forecasting using the ARIMA model.

## Dataset

- **Dataset:** S&P 500 Stock Data
- **File:** `all_stocks_5yr.csv`
- **Source:** [Kaggle – S&P 500 Stock Data](https://www.kaggle.com/datasets/camnugent/sandp500)
- **Description:** Historical stock data for S&P 500 companies, including daily opening, highest, lowest, and closing prices, trading volume, and ticker symbols.

Download the dataset from Kaggle and place `all_stocks_5yr.csv` in the project folder before running the notebook.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Plotly
- Statsmodels
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Data loading and initial inspection
2. Data cleaning and handling missing values
3. Date conversion and chronological sorting
4. Exploratory data analysis
5. AAPL closing-price visualization
6. Candlestick chart visualization
7. Moving-average analysis (20-day and 50-day)
8. Monthly average closing-price analysis
9. Outlier detection using the IQR method
10. Time-series forecasting using ARIMA(5, 1, 0)
11. Model evaluation using MAE, MSE, RMSE, and MAPE
12. Actual versus predicted stock-price comparison

## Forecasting

The notebook focuses on AAPL closing prices and uses a chronological 80:20 train-test split. An ARIMA(5, 1, 0) model is fitted to the training data. Forecasts are compared with actual test values and evaluated using regression error metrics.

The notebook also explores one-step-ahead predictions.

## Repository Contents

- `stock_price_analysis.ipynb` – Analysis and forecasting notebook
- `README.md` – Project documentation
- `requirements.txt` – Required Python libraries

## Author

**Manoj**

[GitHub Profile](https://github.com/Hallada-Manoj)
