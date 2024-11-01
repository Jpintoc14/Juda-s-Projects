VWAP Trade Stats Project

Project Overview

This project analyzes stock trading data using Volume Weighted Average Price (VWAP) as a core metric. By examining top-performing stocks based on VWAP, the project explores trading strategies, backtesting, and visualizing stock movements. The goal is to provide insights into stock performance over time and to backtest strategies using key indicators and trading rules.

Features

VWAP Calculation: Compute the VWAP of stocks and rank them by performance.
Backtesting Simulation: Assess the profitability of trading strategies based on historical data.
Data Visualization: Visualize stock prices and VWAP movements with dynamic charts.
Trading Strategies: Classify stocks based on movement and volatility, and set rules for take-profit (TP) and stop-loss (SL).
Project Structure

VWAP TRADE STATS.ipynb: Jupyter notebook containing all code for data processing, analysis, and visualization.
data/: Contains any datasets used or generated.
README.md: Project documentation.
Installation

Clone the repository and install the necessary libraries:

bash
Copy code
git clone https://github.com/yourusername/vwap-trade-stats.git
cd vwap-trade-stats
pip install -r requirements.txt
Key Libraries
Pandas: Data manipulation and processing.
NumPy: Numerical calculations for data handling.
Matplotlib & Seaborn: Visualization libraries for stock and trading data.
yfinance: Fetch historical stock data.
Scikit-Learn: Used for analysis, feature engineering, and modeling.
ETL Process

Extract: Gather stock data for S&P 500 tickers directly from yfinance.
Transform:
Calculate daily and monthly VWAP for each stock.
Compute percentage price changes and classify stocks based on their price movement and volatility.
Define entry, take-profit, and stop-loss levels based on strategy classifications.
Load: Load transformed data into structures for analysis and plotting.
Usage

Core Functions
Calculate Top Movers: Identifies top-performing stocks by percentage movement.
Classify Strategy: Classifies each stock with strategies such as "Momentum Trading" or "Swing Trading" based on its movement and volatility.
Simulate Trading: Simulates a backtest of each stock’s trading strategy over the last 30 days.
Example Code Snippets
python
Copy code
# Calculate top movers
top_stocks = calculate_top_movers(stock_data)

# Classify trading strategy
strategies = classify_strategy(stock_data, top_stocks)

# Simulate trades based on strategy
results = simulate_trading(stock_data, top_stocks, strategies)
Data Visualization

The project generates various visualizations for analysis:

Stock price trends and VWAP over time.
Distribution of stock movements.
Results of backtested strategies on individual stocks.

