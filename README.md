# Stock Price Analysis and Forecasting using ARIMA

## Project Overview

This project explores historical stock market data using Python, with a focus on Apple Inc. (AAPL). It involves data inspection, cleaning, exploratory data analysis, financial data visualization, outlier detection, and time-series forecasting using the ARIMA model.

The objective is to understand historical stock price movements and evaluate the performance of different forecasting approaches.

## Dataset

- **Dataset:** S&P 500 Stock Data
- **File Name:** `all_stocks_5yr.csv`
- **Source:** [Kaggle – S&P 500 Stock Data](https://www.kaggle.com/datasets/camnugent/sandp500)
- **Description:** Historical stock market data containing daily opening, highest, lowest, and closing prices, trading volume, and stock ticker symbols.

The dataset contains historical records for multiple S&P 500 companies. This project specifically focuses on Apple Inc. (AAPL).

**Note:** Download the dataset from Kaggle and place `all_stocks_5yr.csv` in the same directory as the Jupyter Notebook before running the project.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Plotly
- Statsmodels
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Inspection and Cleaning
- Loaded and explored the stock market dataset.
- Examined data types, dimensions, and statistical summaries.
- Checked missing values and duplicate records.
- Converted the date column into datetime format.
- Removed records with missing OHLC (Open, High, Low, Close) values.
- Sorted records chronologically.

### 2. Exploratory Data Analysis
- Analyzed AAPL closing prices over time.
- Examined long-term stock price trends.
- Calculated 20-day and 50-day moving averages.
- Analyzed average closing prices by month.

### 3. Data Visualization
- Historical closing-price line chart.
- Interactive candlestick chart.
- Moving-average visualization.
- Long-term rolling-average trend.
- Monthly average closing-price bar chart.
- Box plot showing price distribution and outliers.

### 4. Outlier Detection
- Applied the Interquartile Range (IQR) method.
- Calculated Q1, median, Q3, and IQR.
- Identified potential outliers in AAPL closing prices.
- Visualized the distribution using a box plot.

### 5. Stock Price Forecasting using ARIMA

The forecasting analysis focuses on AAPL closing prices.

- Created a chronological 80:20 training and testing split.
- Used an ARIMA(5, 1, 0) model.
- Generated forecasts for the testing period.
- Compared actual and predicted stock prices.

Two forecasting approaches were explored:

**Multi-Step Forecasting**
- The model is fitted using the training dataset.
- Generates predictions for the complete testing period without incorporating actual test observations during forecasting.

**Rolling One-Step-Ahead Forecasting**
- Predicts one observation at a time.
- Incorporates the actual observation into the model before predicting the next observation.
- Evaluates how predictions perform when updated with newly available actual data.

### 6. Model Evaluation

Both forecasting approaches were evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)

Actual and predicted stock prices were also visualized to compare forecasting performance.

## How to Run the Project

1. Clone or download this repository.
2. Download `all_stocks_5yr.csv` from the Kaggle dataset link.
3. Place the CSV file in the same folder as the notebook.
4. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

5. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open `stock_price_analysis.ipynb`.
7. Run the notebook cells sequentially.

## Repository Structure

```text
stock-price-analysis/
│
├── README.md
├── requirements.txt
└── stock_price_analysis.ipynb
```

## Key Learning Outcomes

- Data cleaning and preprocessing using Pandas.
- Exploratory data analysis of financial datasets.
- Financial data visualization using Matplotlib and Plotly.
- Moving-average analysis.
- Statistical outlier detection using IQR.
- Time-series modeling using ARIMA.
- Multi-step and rolling one-step-ahead forecasting.
- Model evaluation using regression error metrics.

## Author

**Manoj**

[GitHub Profile](https://github.com/Hallada-Manoj)
