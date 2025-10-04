# Trading Behavior Analysis & PnL Prediction

## About
This project explores historical trading data and market sentiment to predict whether trades are profitable. It uses feature engineering, machine learning, and visual analysis to understand trading patterns.

## Data
- **Trades**: Daily volume, leverage, number of trades, buy ratio
- **Sentiment**: Fear & Greed Index and classifications (Greed, Fear, etc.)
- **Target**: Closed PnL (log-transformed)

## Project Structure
├── notebooks/ # Jupyter notebooks
├── csv_files/ # Input CSV/PKL files
├── outputs/ # Plots & results
├── ds_report.pdf # Final project report
├── README.md # This file

## Approach
1. Merge and clean trade + sentiment data
2. Engineer features from trading patterns & sentiment
3. Train Random Forest to predict PnL
4. Evaluate using R² and RMSE
5. Future ideas: handle class imbalance (SMOTE/BRF), add temporal features, explore feature importance

## Key Insights
- High/low PnL outcomes happen mainly on high-volume days under Greed/Fear conditions
- Random Forest achieved R² ≈ 0.6 on the test set

## Run
1. Clone the repo
2. Run notebooks in `notebooks/`
3. Plots saved in `outputs/
