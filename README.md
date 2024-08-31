# BTCUSDT Real-Time Trading Signal Bot

This repository contains a Python-based real-time trading signal bot for the BTC/USDT pair using data from Binance's Futures market. The bot streams live market data, processes and analyzes it to generate trading signals, visualizes data using Plotly, and sends notifications along with charts to a specified Telegram channel.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [License](#license)
- [Disclaimer](#disclaimer)

---

## Features

- **Real-Time Data Streaming**:
  - Streams live aggregated trades (`aggTrade`), candlestick data (`kline`), and liquidation orders (`forceOrder`) from Binance Futures WebSocket API.
  
- **Data Processing and Analysis**:
  - Aggregates and processes streamed data to compute metrics such as true volume, false volume, volume difference, and liquidation volume.
  - Generates trading signals (long and short positions) based on predefined volume thresholds and conditions.

- **Data Visualization**:
  - Utilizes Plotly to create interactive and detailed candlestick charts with annotated trading signals.
  - Saves generated charts as images for sharing and record-keeping.

- **Telegram Integration**:
  - Sends instant notifications to a specified Telegram channel/group when trading signals are generated.
  - Shares corresponding chart images alongside textual signal information.

- **Robustness and Reliability**:
  - Implements retry mechanisms and error handling for network requests and WebSocket connections.
  - Supports multi-threading to handle data streaming, processing, and notification tasks concurrently.
  - Automatically attempts to reconnect in case of connection drops or errors.

---

## Prerequisites

- **Python 3.7 or higher**
- **Binance Account**: For accessing Binance Futures data.
- **Telegram Bot Token and Chat ID**: To send notifications via Telegram.

---
## License
This project is licensed under the MIT License.

## Disclaimer
This project is for educational purposes only. Trading cryptocurrencies involves significant risk and can result in financial loss. Use this bot at your own risk. The maintainers and contributors are not responsible for any losses incurred. Always perform due diligence and consider consulting with a professional before engaging in trading activities.

## Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/btcusdt-trading-signal-bot.git
cd btcusdt-trading-signal-bot
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate






