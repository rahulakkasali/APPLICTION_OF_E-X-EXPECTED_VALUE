# APPLICTION_OF_E-X-EXPECTED_VALUE

PROJECT:

>Risk Assessment in Algorithmic Trading Strategies Using Expected Value (ETH)
 >Project Overview
This project implements and evaluates two widely-used algorithmic trading strategies—Moving Average Crossover and RSI Mean Reversion—applied to the cryptocurrency Ethereum (ETH). The primary goal is to analyze the expected returns (
E
(
X
)
E(X)) of these strategies through historical backtesting and probabilistic analysis to better understand risk and performance characteristics.

>Motivation
Quantitative trading heavily relies on balancing risk and reward. Expected value 
E
(
X
)
E(X) provides a foundational statistical measure representing the average expected return, helping traders estimate profitability and risk over repeated trials. Applying this concept to strategies on ETH, a highly volatile but popular crypto asset, offers insights into how these methods might perform in real-world crypto markets.

Data Source

>Historical OHLC (Open-High-Low-Close) data for Ethereum (ETH-USD) from January 1, 2020, to January 1, 2023.

>Data retrieved using the yfinance Python library for easy access to market data.

Strategies Implemented:

1. Moving Average Crossover
>Uses two Simple Moving Averages (SMA): Short-term (10 days) and Long-term (50 days).

>Buy signal when short SMA crosses above long SMA; Sell signal on the reverse crossover.

>Signals captured daily, and trades simulated based on these signals.

2. RSI Mean Reversion

>Computes 14-day Relative Strength Index (RSI).

>Buy signal generated when RSI < 30 (oversold), suggesting price is likely to revert upward.

>Sell signal generated when RSI > 70 (overbought), suggesting price is likely to revert downward.



Methodology:

>Data Preparation:
  >Historical prices cleaned and processed for indicator calculation.

>Indicator & Signal Generation:
 > Calculated SMAs and RSI indicators; generated buy/sell signals accordingly.

>Backtesting Framework:

 >Simulated trades based on signals, calculated daily returns, cumulative returns.

Expected Value Calculation:
>Computed the expected daily return 
E
(
X
)
>E(X) as the average daily return during periods the strategy was active. Annualized returns obtained by scaling daily expected return by ?>trading days.

>Result Visualization:
>Cumulative returns of each strategy plotted over time for visual performance comparison.

Key Outcomes:

>Quantitative comparison of expected returns of two strategies on ETH.

>Insights into strategy behavior under crypto market volatility.

>Foundation for further improvements through parameter tuning or risk management enhancements.

Technologies Used:

>Python 3.9+

>Libraries: pandas, numpy, yfinance, matplotlib

Future works:

>Add more sophisticated risk-adjusted measures like Sharpe ratio.

>Integrate volatility regime segmentation.

>Extend to multiple cryptocurrencies or multi-asset portfolios.

>Implement automated parameter optimization algorithms.


>Environment: Google Colab

