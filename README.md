# Stock Market Price Prediction Using Machine Learning (Python)
# Note: This is in no way a complete nor accurate model and I aim to constantly build upon and improve it as my skills develop.
This project uses historical stock market data from Yahoo Finance to predict short-term price movements using machine learning. It includes a Random Forest classifier model with engineered features such as Relative Strength Index (RSI), trend indicators, and rolling average ratios. The project also features a backtesting framework and capital simulation for evaluating a simple trading strategy.

## Features

- Data loaded directly from Yahoo Finance (using the yfinance library)
- Predicts next-day stock price movement (up/down)
- RandomForestClassifier used to model binary outcomes
- Technical indicators include RSI, price-to-rolling-average ratios, and historical trend strength
- Custom backtesting engine to simulate walk-forward trading
- Strategy logic and capital simulation based on model signals
- Visualisations for RSI, prediction confidence, and equity curve

## Project Objectives

- Investigate short-term predictability of stock prices using supervised learning
- Engineer time-series features that may reveal predictive signals
- Simulate a trading strategy based on model predictions
- Evaluate the financial performance of the strategy under set conditions

## Current Development Status

This project is still in development. I am currently exploring the transition from using a classification approach to a regression-based model (e.g., RandomForestRegressor). The goal is to move beyond predicting only the direction of price movement and instead predict expected percentage returns.

In particular, I am working toward developing a strategy that only enters a trade when the model predicts returns greater than X%, while accounting for uncertainty in the model's output. This should lead to more selective, higher-confidence signals.

I am also evaluating whether the current RandomForestClassifier contributes useful insights or whether it should be replaced entirely when moving to a regression framework. Care is being taken to avoid common time-series data leakage issues that could result in overly optimistic or misleading performance from the machine.
