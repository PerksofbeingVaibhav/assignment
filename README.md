
2. Replace the data collection code in `data_collection.py` with your preferred data source or API to fetch OHLC data for F&O listed stocks in India.

3. Run the `backtesting.py` script to perform the backtest on the 3-year historical data and generate portfolio returns.

4. The `pyfolio_analysis.py` script will analyze the backtest results using Pyfolio and produce a comprehensive performance analysis.

## Data Collection

The `data_collection.py` module is responsible for fetching OHLC data for F&O listed stocks in India. Please replace the data collection code with your data source API or preferred method to collect historical stock data.

## Momentum Strategy

The momentum strategy is implemented in the `momentum_strategy.py` module. It identifies the top 5 performers based on 52-week rolling returns, goes long on these top performers, and sets stop-loss levels at 2 times the ATR on the entry price.

## Backtest and Analysis

The `backtesting.py` script performs the backtest on 3 years of historical data and generates portfolio returns. The `pyfolio_analysis.py` script analyzes the backtest results using Pyfolio, providing insights into the strategy's performance and risk characteristics.

## Disclaimer

Please note that backtesting results do not guarantee future performance. This project is for educational and research purposes only. Always exercise caution and perform thorough testing before implementing any trading strategy in a live environment.

## Contribution

Contributions to the project are welcome! If you find any issues or have suggestions for improvement, feel free to create a pull request or raise an issue in the repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Happy Backtesting and Trading!
            
