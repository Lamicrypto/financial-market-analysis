# Financial Market Analysis & Trading Strategy

## Project Overview

This project analyzes historical Bitcoin market data using Python to evaluate price performance, daily returns, volatility, drawdowns, and risk-adjusted performance.

The project also applies a simple 50-day and 200-day moving average crossover strategy and compares its historical performance against a traditional buy-and-hold approach.

The objective is to demonstrate how data analysis, financial risk metrics, technical indicators, and basic strategy backtesting can be combined to evaluate financial market performance and understand the relationship between investment returns and risk.

> **Disclaimer:** This project is for educational and analytical purposes only. Historical backtest results do not guarantee future performance and do not account for transaction costs, slippage, taxes, liquidity constraints, or market impact.

---

## Project Objectives

The main objectives of this project are to:

* Analyze historical Bitcoin price performance.
* Calculate and evaluate daily returns.
* Measure annualized volatility and rolling volatility.
* Analyze Bitcoin market drawdowns and maximum drawdown.
* Apply 50-day and 200-day moving averages to identify market trends.
* Identify Golden Cross and Death Cross signals.
* Develop a simple moving average crossover trading strategy.
* Compare the historical performance of the strategy against a buy-and-hold approach.
* Evaluate strategies using total return, volatility, maximum drawdown, and Sharpe Ratio.
* Demonstrate how data analysis and financial metrics can support investment strategy evaluation.

---

## Dataset and Data Collection

Historical Bitcoin price data was collected using the `yfinance` Python library.

The analysis focuses on the **BTC-USD** trading pair and covers historical market data from **2020 to 2025**.

The dataset contains historical market information used to analyze Bitcoin's price behavior and includes variables such as:

* Open price
* High price
* Low price
* Closing price
* Trading volume

The analysis primarily focuses on Bitcoin's adjusted closing price for calculating returns, volatility, drawdowns, and technical indicators.

---

## Tools and Technologies

The following tools and technologies were used:

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **yfinance** – Financial market data collection
* **Jupyter Notebook** – Analysis environment
* **VS Code** – Development environment
* **Git and GitHub** – Version control and project management

---

## Methodology

The project followed an end-to-end financial market analysis workflow:

1. Historical Bitcoin market data collection.
2. Data inspection and preparation.
3. Bitcoin closing price analysis.
4. Daily return calculation.
5. Annualized return and volatility analysis.
6. Rolling volatility analysis.
7. Cumulative return and drawdown analysis.
8. Maximum drawdown calculation.
9. 50-day and 200-day moving average analysis.
10. Golden Cross and Death Cross identification.
11. Moving average crossover strategy development.
12. Buy-and-hold and strategy performance comparison.
13. Risk-adjusted performance evaluation using the Sharpe Ratio.

---

## Bitcoin Price Performance

The historical Bitcoin closing price was analyzed to understand the overall price trend during the analysis period.

The analysis demonstrates the significant growth and substantial price fluctuations experienced by Bitcoin between 2020 and 2025.

The historical price visualization provides a foundation for understanding the market cycles and volatility that influenced the subsequent return and risk analysis.

---

## Daily Returns Analysis

Daily percentage returns were calculated to evaluate Bitcoin's day-to-day price movements.

The distribution of daily returns was visualized to understand the frequency and magnitude of positive and negative price changes.

This analysis highlights the highly volatile nature of cryptocurrency markets and provides the foundation for calculating annualized volatility and other risk metrics.

---

## Risk and Volatility Analysis

Volatility was measured to quantify the level of uncertainty and price fluctuation associated with Bitcoin.

The analysis included:

* Annualized volatility.
* 30-day rolling volatility.
* Daily return distribution.

The results demonstrate that Bitcoin experienced substantial volatility throughout the analysis period, highlighting the significant risk associated with cryptocurrency investments.

---

## Drawdown Analysis

Drawdown analysis was used to measure the decline in portfolio value from a previous peak.

The analysis calculated:

* Cumulative returns.
* Running maximum.
* Drawdown.
* Maximum drawdown.

The buy-and-hold approach experienced a maximum drawdown of approximately **-76.63%**, demonstrating the significant downside risk that investors could experience when holding Bitcoin through major market declines.

---

## Technical Analysis

The project applied two commonly used moving averages:

* **50-Day Moving Average (MA50)** – Used to identify shorter- to medium-term price trends.
* **200-Day Moving Average (MA200)** – Used to identify longer-term market trends.

The relationship between these moving averages was analyzed to identify potential changes in Bitcoin's broader market trend.

---

## Moving Average Crossover Strategy

A simple moving average crossover strategy was developed using the 50-day and 200-day moving averages.

### Golden Cross

A Golden Cross occurs when the 50-day moving average crosses above the 200-day moving average.

This was interpreted as a potential bullish trend signal.

### Death Cross

A Death Cross occurs when the 50-day moving average crosses below the 200-day moving average.

This was interpreted as a potential bearish trend signal.

The strategy used the following rules:

* **Position = 1** when MA50 > MA200.
* **Position = 0** when MA50 <= MA200.

The strategy also used a one-day shift on the position signal to reduce the risk of look-ahead bias during the historical backtest.

---

## Strategy Performance Evaluation

The moving average strategy was evaluated against a traditional Bitcoin buy-and-hold approach.

The following metrics were used:

* Total Return
* Annualized Volatility
* Maximum Drawdown
* Sharpe Ratio

### Performance Comparison

| Metric                | Buy and Hold | Moving Average Strategy |
| --------------------- | -----------: | ----------------------: |
| Total Return          |  **855.44%** |             **552.24%** |
| Annualized Volatility |   **60.97%** |              **47.22%** |
| Maximum Drawdown      |  **-76.63%** |             **-56.46%** |
| Sharpe Ratio          |     **0.99** |                **0.96** |

---

## Key Findings

The analysis produced several important findings:

### 1. Buy-and-Hold Generated Higher Historical Returns

The buy-and-hold approach generated a historical total return of approximately **855.44%**, compared with approximately **552.24%** for the moving average strategy.

This indicates that, during the historical period analyzed, remaining invested in Bitcoin produced a higher overall return than the moving average strategy.

### 2. The Moving Average Strategy Reduced Volatility

The moving average strategy recorded annualized volatility of approximately **47.22%**, compared with **60.97%** for the buy-and-hold approach.

This suggests that the strategy reduced exposure to some of Bitcoin's price fluctuations.

### 3. The Moving Average Strategy Reduced Maximum Drawdown

The moving average strategy recorded a maximum drawdown of approximately **-56.46%**, compared with **-76.63%** for buy-and-hold.

This represents a meaningful reduction in historical downside risk.

### 4. Buy-and-Hold Had a Slightly Higher Sharpe Ratio

The buy-and-hold approach achieved a Sharpe Ratio of approximately **0.99**, while the moving average strategy achieved approximately **0.96**.

Therefore, despite the moving average strategy reducing volatility and drawdown, it did not produce a higher risk-adjusted return during the analysis period.

### 5. Return and Risk Involve a Trade-Off

The results demonstrate an important relationship between return and risk.

The buy-and-hold approach generated higher historical returns but exposed investors to substantially greater volatility and drawdowns.

The moving average strategy produced lower historical returns but provided better downside protection and lower overall volatility.

---

## Business and Investment Insights

Based on the historical analysis, several insights can be drawn:

* Investors seeking maximum historical returns during the analyzed period would have benefited more from the buy-and-hold approach.
* Investors more concerned with reducing volatility and downside exposure may find trend-following strategies worth investigating.
* Total return alone is not sufficient for evaluating an investment strategy.
* Maximum drawdown provides important information about the potential severity of losses.
* The Sharpe Ratio can help evaluate whether additional returns adequately compensate for additional risk.
* Technical strategies should be evaluated across multiple market cycles before drawing conclusions about their effectiveness.

---

## Limitations

This project has several limitations:

* The analysis is based on historical Bitcoin price data and does not guarantee future performance.
* The moving average strategy is relatively simple and does not consider other technical or fundamental indicators.
* Transaction costs were not included.
* Trading fees and commissions were not included.
* Slippage was not included.
* Taxes were not included.
* Liquidity constraints were not considered.
* Market impact was not considered.
* The backtest does not account for real-world execution challenges.
* The strategy was evaluated over one historical period and may perform differently under other market conditions.

---

## Project Structure

```text
financial-market-analysis/
│
├── images/
│   ├── bitcoin_historical_closing_price.png
│   ├── bitcoin_daily_return_distribution.png
│   ├── bitcoin_rolling_volatility.png
│   ├── bitcoin_drawdown.png
│   ├── bitcoin_moving_averages.png
│   ├── bitcoin_moving_average_crossovers.png
│   ├── bitcoin_strategy_vs_buy_and_hold.png
│   ├── strategy_return_comparison.png
│   ├── maximum_drawdown_comparison.png
│   └── sharpe_ratio_comparison.png
│
├── financial_market_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## How to Run the Project

### 1. Clone the Repository

Clone the project repository from GitHub to your local machine.

### 2. Navigate to the Project Folder

```bash
cd financial-market-analysis
```

### 3. Install the Required Libraries

Install the dependencies listed in `requirements.txt`.

```bash
pip install -r requirements.txt
```

### 4. Open the Notebook

Open:

```text
financial_market_analysis.ipynb
```

using Jupyter Notebook or VS Code.

### 5. Run the Notebook

Run all cells from beginning to end to reproduce the analysis, calculations, visualizations, and strategy backtest.

---

## Conclusion

This project demonstrates an end-to-end approach to financial market analysis using Python.

The analysis progressed from historical Bitcoin price data and daily return calculations to volatility analysis, drawdown measurement, technical indicators, and trading strategy evaluation.

The results show that the buy-and-hold approach generated a higher historical return during the analysis period, while the moving average crossover strategy provided lower volatility and reduced maximum drawdown.

Although the moving average strategy did not outperform buy-and-hold in terms of total return or Sharpe Ratio during the period analyzed, it demonstrated the potential to reduce exposure to market declines and overall portfolio volatility.

The analysis highlights the importance of evaluating investment strategies using multiple performance metrics, including total return, volatility, maximum drawdown, and Sharpe Ratio.

> **Disclaimer:** This project is for educational and analytical purposes only. Historical backtest results do not guarantee future performance and should not be interpreted as financial advice.

---

## Author

**Balogun Olamide Timothy**

Data Analyst | AI & Machine Learning Enthusiast

Nigeria

**Email:** [olapyperfx24@gmail.com](mailto:olapyperfx24@gmail.com)

**LinkedIn:** https://www.linkedin.com/in/timothy-balogun-0a27192a2

**GitHub:** https://github.com/Lamicrypto

