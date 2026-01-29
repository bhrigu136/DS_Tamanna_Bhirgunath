# Trader Behavior vs Market Sentiment Analysis

This project analyzes the relationship between trader performance and market sentiment
(Fear vs Greed) in the Bitcoin market. The objective is to understand how trading behavior,
risk exposure, and profitability vary under different sentiment regimes.

The analysis combines historical trader data from Hyperliquid with the Bitcoin Fear & Greed Index
to uncover behavioral patterns that can inform smarter trading strategies.


## **Google Colab Notebook:**  
<https://colab.research.google.com/drive/1JpZdAF_N1Syavi6nAig0twrTSlgz4EsH?usp=sharing>
---

## Project Structure:

```

ds_tamanna_bhrigunath/
├── notebook_1.ipynb        # Main analysis notebook (Google Colab)
├── csv_files/              # Cleaned and merged datasets
│   └── merged_trader_sentiment_light.csv
├── outputs/                # Saved plots and visualizations
│   ├── pnl_vs_sentiment.png
│   ├── risk_exposure_vs_sentiment.png
├── ds_report.pdf           # Final summarized insights and conclusions
└── README.md               # Project documentation

```

Note: Large intermediate datasets were excluded from the repository to comply with GitHub file size limits. 
The analysis is fully reproducible using the provided notebook and source data links.

---

## Datasets Used

1. **Bitcoin Fear & Greed Index**
   - Columns: `Date`, `Classification` (Fear / Greed)

2. **Historical Trader Data (Hyperliquid)**
   - Includes trade-level information such as execution price, trade size,
     direction, and closed PnL.

---

## Methodology Overview

- Cleaned and preprocessed both datasets
- Aligned trader data with market sentiment using date-based merging
- Engineered key features such as:
  - Absolute PnL
  - Risk exposure (trade size in USD)
  - PnL efficiency relative to capital
- Performed exploratory data analysis and statistical testing to compare
  trading behavior under Fear vs Greed conditions

Note: Direct leverage data was not available; risk exposure was approximated
using trade size in USD.

---

## Key Insights

- Traders tend to deploy higher capital per trade during Greed phases,
  indicating increased risk appetite.
- Trading activity increases during Greed, suggesting potential overtrading behavior.
- Most trades are breakeven, with overall profitability driven by a small
  number of high-impact trades.
- Market sentiment influences trading behavior more strongly than average profitability.

---

## How to View the Analysis

- Open `notebook_1.ipynb` using Google Colab
- Ensure all folders (`csv_files`, `outputs`) are in the same root directory
- Run the notebook top-to-bottom to reproduce the analysis

All outputs and plots are saved locally within the project structure.

---

## Notes

- All analysis is contained in a single notebook for clarity and cohesion
- Visual outputs referenced in `ds_report.pdf` are stored in the `outputs/` folder
- This project follows the standardized submission format provided in the assignment instructions




