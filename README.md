## Trader Behavior Insights — Radhin Krishna

This repository presents an in-depth analysis of how trader behavior aligns with market sentiment, with a focus on historical trading patterns and Bitcoin’s Fear & Greed Index.

###  Project Structure

- **`csv_files/`**  
  Contains the core datasets used in this project:  
  1. **Bitcoin Market Sentiment Dataset** — Columns: `Date`, `Classification` (e.g. Fear, Greed)  
  2. **Hyperliquid Trader Data** — Columns: `account`, `symbol`, `execution price`, `size`, `side`, `time`, `start position`, `event`, `closedPnL`, `leverage`, etc.

- **`Output/`**  
  Stores all visual assets including plots, charts, and dashboards (`.png`, `.jpg`).

- **`Trader Behavior Insights.ipynb`**  
  Interactive notebook containing EDA, time-series trends, statistical testing, and strategic takeaways.

###  Key Analyses & Findings

#### 1. Time Series Insights
- Daily **Average PnL** segmented by sentiment classification.
- Total traded volume patterns across time.
- 7-Day moving average for Avg PnL.
- Calendar heatmaps visualizing Total PnL for 2024–2025.

#### 2. Statistical Testing
- **ANOVA test**: No significant difference found across sentiment classes (p = 0.8458).
- **Tukey’s HSD**: Post-hoc tests showed no statistically significant differences between sentiment pairs.

#### 3. Interpretation Highlights
- Largest Avg PnL difference seen between *Extreme Greed* and *Extreme Fear* (~$37.88), though not statistically significant.
- High variance and wide confidence intervals suggest inconsistent profitability across sentiment types.
- All p-values > 0.84 imply weak correlation between sentiment and trading outcomes.

#### 4. Recommendations
- Incorporate additional features like volatility, weekday patterns, and rolling stats to enrich predictive models.
- Reevaluate sentiment classifications using binary or multi-level binning.
- Expand the dataset for stronger signal detection and pattern reliability.
