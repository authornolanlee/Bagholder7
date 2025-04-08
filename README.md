# The Bagholder 7 📉💼 (aka BAG7 or BAGnificent 7)

This fund selects 7 high-conviction stocks for aspiring bagholders. This is for entertainment purposes only and does not constitute investment advice.

A dynamic HTML-based portfolio tracker designed to visualize performance over time. Built with Chart.js and powered by Yahoo Finance data via a CORS proxy.

## 🚀 Features

- Track portfolio value across time
- Visual rebalance points on the chart
- Compare to benchmark indices (S&P 500, NASDAQ, DJIA)
- Toggle between % return and dollar value views
- Customize Y-axis min/max values
- View current holdings and full portfolio history

## 📊 Example Portfolio History

| Date       | Allocation                                 | Value |
|------------|---------------------------------------------|----------|
| 2025-01-01 | 15% MSTR, 15% SAVA, 15% QBTS, 15% IONQ, 15% RGTI, 15% RIVN, 10% AMC  | $10,000.00 | 


## 🛠 Setup

You can load the page by visiting [github.io](https://nickaustinlee.github.io/Bagholder7/). 

If you want to change the portfolio into your own Bagholder 7 selection, here is how you do it:

1. Clone this repo or download the HTML file.
2. Open `index.html` in your browser (no build steps needed).
3. Update the `portfolioDataNDJSON` block in the HTML to match your investment timeline.

## 📎 Data Format (NDJSON)

Note: You can change allocations on any date, but I suggest checking the last trading day's value and ensuring the dollar value is preserved for your new allocation.

```json
{"Tickers": ["MSTR", "SAVA", "QBTS"], "Proportions": [0.25, 0.25, 0.5], "Dollars": 1000, "Date": "2025-01-01"}
{"Tickers": ["MSTR", "SAVA", "QBTS"], "Proportions": [0.3, 0.4, 0.3], "Dollars": 800, "Date": "2025-02-01"}
