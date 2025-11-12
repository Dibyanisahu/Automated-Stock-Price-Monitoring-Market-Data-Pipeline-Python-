🧭 **Stock Market Price Tracker using Python**

A Python-based real-time stock tracker that fetches live and historical prices from Yahoo Finance, while intelligently accounting for Indian stock market hours (BSE/NSE), weekends, and public holidays.

This project automates stock price fetching at user-defined times and intervals, making it a valuable tool for data analysts, investors, and finance enthusiasts who want to monitor price trends or integrate data into analytics dashboards.


**🚀 Features**

✅ Fetches live and historical stock data from Yahoo Finance

✅ Supports NSE/BSE-listed stocks (e.g., ZOMATO.NS, TVSMOTOR.BO)

✅ Adjusts for market hours: 9:15 AM – 3:30 PM IST (Mon–Fri)

✅ Skips weekends and national holidays automatically

✅ Provides nearest available market price if queried outside trading hours

✅ Handles minute-level, hourly, or daily intervals dynamically

✅ Displays clean, formatted output with time offset comparisons



**🧩 Tech Stack**

Python 3.10

yfinance – to fetch stock prices

pandas – for data manipulation

pytz – for timezone handling

holidays – for dynamic market holiday checks


**🧮 How It Works**

Input a stock ticker (e.g., ZOMATO.NS or TVSMOTOR.BO).

Enter a specific date and time — the tracker adjusts automatically if the market is closed.

The script fetches the nearest available price from Yahoo Finance.

Compares time offsets like +1 minute, +5 minutes, +1 hour, and +1 day for analysis.


**🕒 Market Logic**
Exchange	Open Time (IST)	Close Time (IST)	Days
BSE/NSE	9:15 AM -	3:30 PM,	Mon–Fri

Automatically skips weekends and public holidays (using the holidays package).

Adjusts requests outside market hours to the next valid trading session.


**💻 Installation**
# Clone the repository
On Windows: open Git Bash (installed with Git).
On macOS/Linux: open Terminal.

Clone command:
git clone https://github.com/Dibyanisahu/Automated-Stock-Price-Monitoring-Market-Data-Pipeline-Python-.git



# Install dependencies
pip install -r requirements.txt



**requirements.txt**

pandas
yfinance
pytz
holidays


**🧠 Usage**
python stock_tracker.py



**Example Interaction:**

Enter stock ticker (e.g., ZOMATO.NS): ZOMATO.NS
Enter date (DD Mon YYYY): 05 Nov 2025
Enter time (HH:MM, 24-hour): 12:30

The stock prices of ZOMATO.NS for requested date and time are:
------------------------------------------------------------
Time Offset |   Market Time     |              Price (INR)
------------------------------------------------------------
Base Time  ,    05 Nov 2025 12:30    ,       177.25 |
+1 Hour    ,    05 Nov 2025 13:30    ,        178.10|
+1 Day     ,    06 Nov 2025 12:30    ,        179.35|
------------------------------------------------------------


**🧩 Example Use Cases**

Automate daily stock price tracking and save to CSV/Excel.

Build interactive dashboards in Tableau or Power BI using price data.

Backtest trading strategies using historical data.

Monitor market performance of specific companies.


**📊 Future Enhancements**

🔹 Add price alerts via email or Telegram.
🔹 Integrate with Google Sheets API for daily logs.
🔹 Add portfolio tracking and visualization.

**👤 Author**

Dibyani Sahu
Data Scientist passionate about building practical Python automation tools for analytics and financial insights.
