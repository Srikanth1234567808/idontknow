📊 Quantitative Trading Strategy Engine
This project is a fully automated backtesting engine designed to:

📈 Download historical stock data

⚙️ Generate random rule-based trading strategies using technical indicators

🧪 Backtest those strategies

🏆 Select and log the best-performing strategies based on Sharpe ratio

🔄 Export trade signals and results to Google Sheets

🚀 Features
✅ Data download via Yahoo Finance using yfinance

📐 Technical indicators via pandas_ta

🎲 Randomized strategy generation using common indicators like RSI, MACD, SMA, EMA

🧠 Backtesting with signal logic and performance metrics (Sharpe Ratio & Cumulative Return)

📁 Exports top strategies to CSV

🧾 Trade logs and performance summaries directly written to Google Sheets

🧪 Technical Indicators Used
Relative Strength Index (RSI)

Simple Moving Averages (SMA)

Exponential Moving Averages (EMA)

MACD (Moving Average Convergence Divergence)

.
├── strategy_engine.py         # Main script
├── top_strategies.csv         # Generated after run (if saved)
├── secret-cipher-*.json       # Your Google service account credentials

🔐 Google Sheets Setup
Create a Google Cloud project and enable Google Sheets & Drive API.

Create a Service Account and download the credentials JSON.

Share your target Google Sheet with the service account email (xyz@project.iam.gserviceaccount.com).

Replace the default credential path in run_algo() with your JSON file path.

📊 Output
top_strategies.csv — Top N strategies sorted by Sharpe ratio

Google Sheet:

Trade_Log: Signals where trades would have been placed

Summary: All strategy results (cumulative return + Sharpe ratio)

Win_Ratio: Total strategies, number of winners, and win ratio
