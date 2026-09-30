# Why India's Economy Grows While Its Stock Market Falls

A finance project that explains why India's GDP can grow quickly while the Nifty falls, using Python analysis in Google Colab and a written report.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubha0010/India_Economy_vs_Stock_Market/blob/main/India_Economy_vs_Stock_Market.ipynb) 

> 

## The question

India's GDP grew 7.8% last quarter, ahead of the RBI's 7.0% forecast, yet the Nifty is about 14% below its peak. Can the data explain this gap?

## Main argument

1. **Different clocks.** GDP reports what has already happened. Stock prices reflect expected future earnings.
2. **Foreign selling.** Foreign investors sold the biggest Nifty stocks, while domestic SIP money mostly went into mid- and small-cap funds.
3. **Weak index earnings.** Nifty earnings grew only in low single digits for two years against expectations of double digits.
4. **Concentration.** Financials and IT make up about 45% of the Nifty, and three stocks (HDFC Bank, ICICI Bank, Reliance) carry about 27%.
5. **Index mismatch.** Growth sectors such as electronics and capital goods have almost no weight in the Nifty.

The US shows the reverse case: a slowing economy with record-high stocks, driven by a few giant companies.

## What is in this project

| File | Description |
|---|---|
| `India_Economy_vs_Market_Project.ipynb` | Google Colab notebook with the full analysis |
| `economy_vs_market_report.html` | Written report with charts and findings |
| `README.md` | This file |

## Notebook structure

| Part | What it does | Data source |
|---|---|---|
| A | Loads the key figures and charts them | YouTube video by The Valuation School (Parth Verma) |
| B | Contribution analysis: how a few heavyweights drag the index (`weight x return`) and a sensitivity chart | YouTube video by The Valuation School (Parth Verma), plus editable assumptions |
| C | Drawdowns from peak and growth-of-100 comparison of the Nifty, sector indices, heavyweights and non-index winners | Yahoo Finance via `yfinance` |
| D | Correlation and regression between yearly GDP growth and yearly Nifty returns | World Bank API and `yfinance` |

## How to run

1. Open the notebook in Google Colab using the badge above, or upload the `.ipynb` file at [colab.research.google.com](https://colab.research.google.com).
2. Choose **Runtime → Run all**.
3. Parts C and D need an internet connection, which Colab provides.

Libraries used: `pandas`, `numpy`, `matplotlib`, `scipy`, `requests`, `yfinance`.

## Limitations

- Part B uses **assumed** individual weights and an assumed return for ICICI Bank. The source gives only the combined ~27% weight and a "25%+" fall for HDFC Bank and Reliance. Edit the values to match current data.
- Part D uses a small number of annual data points, and it tests same-year relationships only. Markets often move ahead of the economy, so a lagged analysis could give different results.
- Live data from Yahoo Finance can have gaps or change ticker symbols. Results depend on the date you run the notebook.
- Figures from the YouTube video reflect its publication date.

## Sources

- The Valuation School (hosted by Parth Verma), YouTube video, thevaluationschool.com
- Yahoo Finance, accessed through the `yfinance` library
- World Bank Open Data, indicator NY.GDP.MKTP.KD.ZG (India GDP growth)

## Disclaimer

This project is for educational purposes only and is not investment advice.

## Author

**SHUBHA HALDER**
