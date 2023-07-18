# Momentum Strategy Backtest for F&O Listed Stocks in India

This repository contains a Python project to test the momentum strategy on F&O listed stocks in India. The strategy involves going long on the top 5 performers based on 52-week rolling returns and setting a stop loss at 2 times the Average True Range (ATR) on the entry price. The portfolio will be rebalanced on a weekly basis.

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Setup and Usage](#setup-and-usage)
- [Data Collection](#data-collection)
- [Momentum Strategy](#momentum-strategy)
- [Backtest and Analysis](#backtest-and-analysis)
- [Disclaimer](#disclaimer)
- [Contribution](#contribution)
- [License](#license)

## Introduction

The Momentum Strategy is a popular trading strategy that aims to capitalize on the continuation of trends in stock prices. This project tests the effectiveness of the momentum strategy on F&O listed stocks in India over a period of 3 years.

## Project Overview

- `data_collection.py`: This module contains functions to fetch OHLC (Open, High, Low, Close) data of F&O listed stocks in India from a data source.

- `momentum_strategy.py`: The core of the project, where the momentum strategy is implemented. It includes a custom function to identify the top 5 performers based on 52-week rolling returns, buying the top performers, and setting stop-loss levels using 2 times ATR.

- `backtesting.py`: This script performs the backtest on the 3-year historical data and generates portfolio returns.

- `pyfolio_analysis.py`: The analysis script that uses the Pyfolio library to analyze the backtest results, providing performance metrics, risk analysis, and visualizations.

## Setup and Usage

1. Install the required Python packages by running the following command:
pip install -r requirements.txt

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
