# Python Portfolio Tracker

Currently a work in progress...🏗️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
[![codecov](https://codecov.io/gh/julian-west/python_portfolio_tracker/branch/master/graph/badge.svg)](https://codecov.io/gh/julian-west/python_portfolio_tracker)

Track the performance of your portfolio using Python!

## Problems this repo solves

Online broker accounts tend to give generalised statistics about portfolio (or individual stock) performance. It can be difficult to easily download any source data to do your own in depth analysis on the performance of any individual positions and the overall risk return profile of the portfolio. Furthermore, if you have accounts with multiple brokers it is very difficult and time consuming to complete an analysis of all your positions.

Using a simple list of buy/sell positions in a csv file as input, this repo aims to allow the user to efficiently collect daily stock price data, calculate the value of their portfolio over time and complete custom in depth analysis of positions (e.g mean-variance, correlations, etc.).a

## How to use

// TODO

### Data Input Format

//TODO

## Current limitations

- Data processing and analysis is completed in memory which may not scale we to portfolios with many different positions
- Stock price data is loaded from `yahooFinance` (using the `ffn` library), the veracity of this data source may not be 100% and it can also take a long time to load data

## Running Tests

PyTest is used for running tests in this project. In order to run tests, run the following command in the project directory (make sure libraries in test_requirements.txt are installed):

```bash
pytest --cov-config=.coveragerc --cov=src
```

## Further work

- User input through webapp rather than csv/Jupyter Notebooks
- Account for dividend payments
