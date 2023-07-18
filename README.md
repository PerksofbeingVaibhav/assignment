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
