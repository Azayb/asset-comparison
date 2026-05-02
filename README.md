link: https://github.com/Azayb/asset-comparison

# Cross-Asset Comparison Charts

Built by an undergraduate student interested in global markets. This dashboard tracks 20 financial instruments across equities, rates, credit,
commodities, FX, and volatility to monitor cross-asset market dynamics in real time.

Disclaimer: This is an ongoing project of mine. The code is complete, but the market analysis and conclusions I am drawing from it are still
incomplete. I run it regularly to track how markets are developing and will continue updating my findings as I work through each chart and as
new data comes in.

---

## Charts

### Asset Class Performance Individually
<img width="868" height="468" alt="Screenshot 2026-05-02 at 3 47 26 PM" src="https://github.com/user-attachments/assets/7b861590-ca8c-45ca-98b0-1f0d61ba68d2" />


### Asset Class Performance by Group

<img width="728" height="587" alt="Screenshot 2026-05-02 at 3 48 14 PM" src="https://github.com/user-attachments/assets/161492fb-c027-45a3-8c2c-07166ed5796c" />

### Asset Class Comparison (Group Averages)

<img width="728" height="372" alt="Screenshot 2026-05-02 at 3 48 57 PM" src="https://github.com/user-attachments/assets/69e09c9b-226c-4b22-aab0-8757cbeed66b" />


### Cross-Asset Correlation Matrix

<img width="591" height="460" alt="Screenshot 2026-05-02 at 3 49 25 PM" src="https://github.com/user-attachments/assets/3e7ecdc9-b196-4b5c-b403-dd66bea1ffb9" />


---

## Assets Tracked

| Asset Class | Instruments |
|-------------|-------------|
| Equities | S&P 500, Nasdaq 100, Russell 2000, Emerging Markets |
| Rates | 1-3Y Treasury, 7-10Y Treasury, 20Y+ Treasury |
| Credit | High Yield Credit, Investment Grade Credit |
| Commodities | Gold, Silver, Oil, Broad Commodities |
| FX | US Dollar Index, Euro, Japanese Yen, Canadian Dollar |
| Sectors & Vol | Financials, Energy, Volatility Proxy |

---

## Features
- Normalized performance chart comparing all 20 assets on equal footing
- Asset class group comparison showing relative performance across 6 categories
- 20-day rolling volatility dashboard tracking real-time risk across all asset classes
- Cross-asset correlation heatmap identifying diversification and hedging relationships
- Summary statistics table ranking all assets by total return, volatility, Sharpe ratio, and max drawdown

---

## Key Findings (May 2025 - May 2026)

Commodities performed best, with silver in the lead
 - Silver returned +136% and Gold +67%, outperforming every other asset class. Silver's surge was driven by both safe-haven demand and
 - industrial use. Gold benefited investors shifting away from the dollar as their go-to safe haven.

The Dollar lost its safe-haven status to Gold
 - The US Dollar and VIX used to have a positively correlated relationship prior to this year. This year, the dollar stayed flat while volatility fell, and gold surged instead. With tariffs and political uncertainty making the dollar less reliable, investors turned to gold instead.

Oil spiked due to the Iran war
 - Oil was relatively stable for most of the year until March 2026 when the Iran war began. Iran controls the Strait ofe Hormuz, where roughly 20-25% of global oil supply passes. When the strait closed, supply was disrupted, and prices spiked. Since then, oil has been volatile, rising and falling with each development in the war, but overall remaining elevated. 

The Japanese Yen weakened all year
 - The Yen declined due to the interest rate gap between Japan and the US. The US currently has a borrowing rate of 3.75% while Japan’s is 0.75%. Investors borrow cheaply in Yen and invest in higher-yielding US assets (known as the carry trade), which kept consistent selling pressure on the Yen throughout the year. This does give Japan a trading advantage, as it pushes Japanese residents to purchase domestically, hurting foreign companies that sell to Japan. 

VIXY fell despite occasional fear spikes
 - According to past articles, VIX was low ending 2025 largely due to strong corporate earnings, AI-led growth, and the recession that many predicted never arriving. By early 2026, articles began questioning whether massive AI investments were actually paying off, which started pushing volatility back up. VIXY did experience brief spikes, mostly during last year's tariff shock and the March 2026 Iran war.

Bonds and Stocks Relationship is changing
 - SPY and 10Y Treasuries showed almost zero correlation over the past year. The traditional relationship, where bonds go up when stocks go down, has broken down and apparently has been since 2022. *currently researching the reasons behind this shift and will 
update findings as I learn more*


## Tech Stack
- **Python 3.14**
- **pandas** — data manipulation, returns calculation, rolling metrics
- **yfinance** — live market data pulled directly from Yahoo Finance
- **plotly** — interactive charts
- **Jupyter Notebook** — development environment

---


## How To Run
```bash
git clone https://github.com/Azayb/asset-comparison.git
cd asset-comparison
python3 -m venv venv
source venv/bin/activate
pip install yfinance pandas matplotlib plotly notebook
jupyter notebook asset_comparison.ipynb
```

---


## What I Learned
- How to pull and clean real financial market data using Python
- How to calculate daily returns, rolling volatility, Sharpe ratios, and max drawdown
- How to read cross-asset signals to identify risk-on vs risk-off market environments
- How to think about correlation as a tool for diversification and hedging
- Analyzing the relationships between different assets and asset classes and drawing independent conclusions. 

## Note
This program was built to collect the past 1 year of closing prices for 20 instruments spanning the major asset classes: equities, fixed
income, credit, commodities, FX, and volatility. Using daily returns, the analysis examines performance, volatility, and correlation across
assets, both individually and by asset class, to identify broader market trends and relationships. A summary statistics table ranks assets by
total return, current volatility, and risk-adjusted return in order to compare not just how much each asset returned, but the risk associated
with each asset's return. The goal was to draw my own conclusions from the past year's data rather than just reading about them, allowing me to
better understand the relationship between assets, build intuition for how specific assets move, and overall strengthen my knowledge of the
markets.

.
.
.
.
.
.
.
.
.
___
.
.
.
.
.
.
.
.
.

