SPY Weekly Prices Analysis

This repository contains Jupyter notebooks that analyze weekly price data for the SPY ETF (S&P 500 ETF Trust). The analysis focuses on calculating key technical indicators, generating visualizations, and exploring potential trading strategies based on these indicators.

Files in this Repository

1. `SPY_Weekly_Prices (1).ipynb`
   - Purpose: This notebook loads weekly SPY price data, calculates key moving averages, and provides an exploratory data analysis (EDA) of SPY's historical price movements.
   - Features:
     - Loads SPY data and formats the date for readability.
     - Calculates important technical indicators, such as the Exponential Moving Average (EMA) and Simple Moving Average (SMA).
     - Visualizes price trends with candlestick charts and overlays of calculated indicators.
     - Provides foundational data and insights for understanding SPY's weekly trends and historical performance.
2. `weekly_spy_data2 (1).ipynb`
   - Purpose: This notebook builds on the exploratory data by implementing a basic trading strategy based on moving average crossovers.
   - Features:
     - Implements a trading algorithm where:
       - A buy signal is generated when the 50-day SMA crosses above the 21-day EMA.
       - A sell signal is triggered when the 21-day EMA crosses above the 50-day SMA.
     - Records trade entry and exit points, including:
       - Entry and exit dates.
       - Entry and exit prices.
       - Calculated profit or loss (PnL) for each trade.
     - Provides a summary of trades based on the crossover strategy, including cumulative returns.

Requirements

- Python 3.8+
- Jupyter Notebook
- Libraries:
  - `pandas` for data manipulation.
  - `plotly` for data visualization, especially candlestick charts.
  - `numpy` for numerical operations.

To install the required packages, you can use:

```bash
pip install pandas plotly numpy
```

Getting Started

1. Clone the Repository:

   ```bash
   git clone https://github.com/Shelton-beep/trading-algorithm.git
   cd trading-algorithm
   ```

2. Open the Jupyter Notebooks:
   Launch Jupyter Notebook in the project directory to access the notebooks:

   ```bash
   jupyter notebook
   ```

   Open `SPY_Weekly_Prices (1).ipynb` for data exploration and visualization, or `weekly_spy_data2 (1).ipynb` for the trading strategy implementation.

3. Run the Notebooks:
   Follow the code cells in each notebook sequentially to load data, process indicators, and generate visualizations or trading signals.

Project Goals

This project aims to:

- Provide an overview of SPY’s historical weekly price movements.
- Develop a basic trading algorithm based on moving average crossovers.
- Demonstrate the impact of technical indicators on trading strategies.

Future Work

Planned improvements include:

- Backtesting additional technical indicators.
- Optimizing the strategy with different moving average windows.
- Incorporating risk management techniques.
