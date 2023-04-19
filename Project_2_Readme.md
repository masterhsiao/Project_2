## Overview:

**This project presents a long-only trading strategy that combines technical analysis with risk management to identify potentially undervalued stocks and generate buy signals. The strategy employs Bollinger Bands and Relative Strength Index (RSI) as indicators to generate buy signals, and Average True Range (ATR) to set a trailing stop loss.** 

### Technical Indicators:

**Bollinger Bands:**

> Bollinger Bands are a technical indicator that measure the volatility of a stock's price relative to its moving average. The bands are created by calculating the standard deviation of the stock's price over a certain number of periods and adding or subtracting this value from the moving average. The bands provide a visual representation of the price volatility, with the bands expanding when the stock is volatile and contracting when the stock is less volatile.

**Relative Strength Index (RSI):**

> The RSI is a momentum indicator that measures the strength of a stock's price action by comparing the magnitude of recent gains to recent losses. The RSI ranges from 0 to 100, with a reading above 70 indicating an overbought stock and a reading below 30 indicating an oversold stock.

**Average True Range (ATR):**

> The ATR is a technical indicator that measures the volatility of a stock's price by taking into account the range of price movements over a certain number of periods. The ATR is used to set the trailing stop loss, which is a way to limit potential losses in a trade by automatically selling the stock if the price drops below a certain level.
---
### Trading Strategy: Trailing Stop Loss

The trading strategy aims to identify stocks that are potentially undervalued and poised for a rebound. The strategy combines technical analysis using Bollinger Bands and RSI to generate buy signals and risk management using ATR to set a trailing stop loss.

The buy signals are generated when the stock's price crosses above the upper Bollinger Band and the RSI is below a certain threshold, indicating that the stock is oversold and potentially undervalued. When a buy signal is generated, the script will initiate a long position in the stock.

The trailing stop loss is set at a certain multiple of the ATR. This means that if the stock's price drops by more than the ATR multiple from its peak, the script will automatically sell the stock to limit potential losses.

### Performance Metrics:

The script calculates various performance metrics, including the total return, annualized return, win rate, and more. These metrics are used to evaluate the effectiveness of the trading strategy and to make improvements if necessary.

### Installation Instructions:

 To use this trading strategy, you will need to have Python 3 installed on your machine along with the following libraries:

1. alpaca_trade_api
2. finta
3. scikit-learn
4. pandas
5. numpy
6. matplotlib
You can install these libraries using pip by running the following command:

`pip install alpaca_trade_api finta scikit-learn pandas numpy matplotlib`

Usage Instructions:

**To use this trading strategy, follow these steps:**

Clone the repository or download the files to your machine.
Open the trading_strategy.py file in your preferred Python editor or environment.
Replace the API_KEY and SECRET_KEY variables with your Alpaca API credentials.
Set the TICKER variable to the stock you want to trade.

Run the XXXXXXXXXXXXXXXX.py file.

The script will retrieve historical stock data for the specified ticker, calculate the necessary indicators, and generate buy signals based on the strategy described above. The script will then simulate trades and calculate performance metrics.

 **Note:**

This trading strategy is for educational purposes only and should not be used for actual trading without proper backtesting and risk management. The author of this project is not responsible for any losses incurred from using this strategy.