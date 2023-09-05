# Crypto Trading Bot Simulation with Streamlit

##Deployed app link: https://trading-bot-2esbr29hycqzyxshkdets7.streamlit.app/

## Overview

This project is a Python-based simulation of a cryptocurrency trading bot using the Streamlit framework. It allows users to configure and run a simple trading strategy and observe the bot's actions and account balance in real-time. 

## Objective

The objective of this project is to create a user-friendly interface for simulating cryptocurrency trading strategies. It's intended for educational and demonstrative purposes only and should not be used for actual trading.

## Key Features

1. **Streamlit Interface:** The project uses Streamlit, a Python library for creating web applications with minimal code, to build a user interface for configuring and running the trading bot.

2. **Bot Configuration:** Users can configure various settings of the trading bot, including the bot's speed (how frequently it makes decisions), the initial account balance in USDT (US Dollar Tether), the trading pair (e.g., BTC/USDT), and the short and long windows for moving average calculations.

3. **Display of Bot Configuration:** The selected bot settings are displayed in a sidebar to provide transparency and help users keep track of the chosen parameters.

4. **Start and Stop Buttons:** The "Start Bot" and "Stop Bot" buttons allow users to control when the bot runs. Clicking "Start Bot" initiates the bot's execution, while "Stop Bot" halts its operation.

5. **Bot Logic:** The bot fetches historical cryptocurrency price data from the CryptoCompare API and calculates two simple moving averages (SMA) based on the user-defined short and long windows. It then implements a basic crossover strategy:
   - When the short-term SMA crosses above the long-term SMA, it triggers a "Buy" signal.
   - When the short-term SMA crosses below the long-term SMA, it triggers a "Sell" signal.
   - Otherwise, it's in a "Hold" state.

6. **Output Display:** The bot's actions, including buy/sell signals and changes in the account balance, are displayed in real-time in the main content area. This provides users with clear feedback on the bot's decisions.

7. **Realistic Account Balance:** The bot maintains a hypothetical account balance in USDT, and the balance is adjusted based on executed buy and sell orders.

## Usage

- Users can adjust bot settings and click "Start Bot" to initiate the simulation.
- The bot will continuously fetch data, calculate SMAs, and execute buy/sell orders based on the defined strategy.
- Users can click "Stop Bot" to halt the bot's execution at any time.

## Note

- This project is purely for educational and demonstrative purposes. It does not connect to any real cryptocurrency exchange or execute actual trades.
- Users should use their discretion and not rely on this simulation for real trading decisions.

## Enhancements

This project can be further enhanced by adding more sophisticated trading strategies, integrating real-time data from a live exchange via API, and conducting backtesting of strategies against historical data.

## Disclaimer

This project is not intended to provide financial or investment advice. Cryptocurrency trading carries inherent risks, and users should exercise caution and conduct thorough research before engaging in actual trading.

