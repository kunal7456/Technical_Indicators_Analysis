Trading Strategies Analysis :

This project provides Python code to analyze and implement various trading strategies using financial data obtained from Yahoo Finance. The strategies implemented include:

Relative Strength Index (RSI) Strategy:

Calculation of RSI:

Initialize Average Gain (AG) and Average Loss (AL) for the first 14 periods.

Calculate daily gains and losses over the next 14 periods.

Compute Average Gain and Average Loss.

Calculate Relative Strength (RS) and RSI using the formulas.

Signal Generation:

Buy when RSI is below 30.

Sell when RSI is above 70.

Returns Calculation:

Evaluate returns based on generated buy/sell signals.

Moving Average Convergence Divergence (MACD) Strategy:

Calculation of MACD:

Calculate Short-Term Exponential Moving Average (ShortEMA) and Long-Term Exponential Moving Average (LongEMA).

Compute MACD line by subtracting LongEMA from ShortEMA.

Calculate the Signal Line using the MACD line.

Derive the MACD Histogram as the difference between MACD and Signal Line.

Signal Generation:

Buy when MACD crosses above the Signal Line.

Sell when MACD crosses below the Signal Line.

Returns Calculation:

Evaluate returns based on generated buy/sell signals.

Bollinger Bands (BB) Strategy:

Calculation of Bollinger Bands:

Compute Simple Moving Average (SMA) over a 14-day period.

Calculate Standard Deviation (STD) over the same 14-day period.

Determine Upper Band (BU) and Lower Band (BL) as SMA ± (2 * STD).

Signal Generation:

Buy when the closing price crosses below the Lower Band.

Sell when the closing price crosses above the Upper Band.

Returns Calculation:

Evaluate returns based on generated buy/sell signals.

Mixed Strategy:

Signal Generation:

Combine signals from MACD and Bollinger Bands.

Buy when MACD and closing price conditions are met.

Sell when Bollinger Bands conditions are met.

Returns Calculation:

Evaluate returns based on generated buy/sell signals.

Instructions:

Prerequisites:

Install necessary Python packages using the provided requirements.txt file.

Usage:

Run the script trading_strategies.py.

Analyze the generated plots for each strategy and observe the buy/sell signals.

Check the calculated returns for each strategy.

Code Structure:

trading_strategies.py: Main script containing functions for downloading financial data, calculating indicators, generating signals, and evaluating returns.

Data Sources:

Financial data is obtained from Yahoo Finance using the yfinance library.

NSE and SSE indices data is fetched using the nsetools library.

Dependencies:

yfinance

nsetools

numpy

pandas

matplotlib

scipy
