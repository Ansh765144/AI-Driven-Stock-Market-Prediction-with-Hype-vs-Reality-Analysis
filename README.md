# AI-Driven-Stock-Market-Prediction-with-Hype-vs-Reality-Analysis

## Overview
This project presents a machine learning-based framework for stock price prediction combined with sentiment-driven behavioral analysis.
The system predicts next-day closing prices using engineered financial indicators and evaluates whether market sentiment (hype) aligns with actual price movement.
The goal is not just prediction — but understanding when hype matches reality and when it fails.

## Problem Statement
Stock markets are influenced by both technical indicators and investor sentiment.  
Traditional models focus only on price trends and ignore behavioral hype effects.
This project addresses:
- Can we accurately predict next-day stock prices?
- Does market sentiment actually reflect real price movement?
- How often does hype fail?

## Companies Used
- TCS
- INFY
- RELIANCE
- SBIN
Data Source: National Stock Exchange (NSE)
Time Range:
- Training: 2020–2025
- Future Validation: Jan–20 Feb 2026

## Methodology
### 1️⃣ Feature Engineering
Created technical indicators including:
- Daily Return
- Price Change
- Moving Averages (MA-3, MA-7)
- Lag Features
- Sentiment Score & Counts

### 2️⃣ Model Used
- Random Forest Regressor
- Time-series safe training (no shuffle)
- Ensemble learning for nonlinear financial patterns

### 3️⃣ Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Percentage Error
- Visual validation plots

## Results
- R² Score (Future Validation): ~0.999
- Average Percentage Error: ~1.07%
- Strong alignment between predicted and actual prices
The high accuracy is influenced by:
- Effective feature engineering
- Structured financial dataset
- Ensemble robustness of Random Forest

## Hype vs Reality Analysis
A behavioral module was introduced to compare:
Sentiment Expectation vs Real Market Direction
Categories:
- Hype Correct
- Hype Failed
- Neutral Impact
This helps identify cases where investor sentiment diverges from actual market movement.

## Key Insights
- High predictive performance on structured time-series data
- Sentiment does not always reflect real market behavior
- Combining ML + behavioral validation improves interpretability

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## Limitations
- Dataset limited to 4 companies (not cross-sector or global scale)
- Short-term next-day prediction only
- High R² influenced by structured dataset and limited prediction horizon
- Random Forest does not model deep sequential time dependencies (like LSTM)
- Sentiment analysis based on aggregated scores (not deep contextual NLP)
- Does not account for sudden macroeconomic or geopolitical shocks
- Model not yet optimized using systematic hyperparameter tuning

## Future Improvements
- Compare with XGBoost / LSTM
- Add cross-validation
- Real-time sentiment scraping
- Hyperparameter tuning optimization
## Author
Ansh Uniyal  
MTech Integrated CSE
Noida Institute Of Engineering and Technology, Greater Noida, Uttar Pradesh, India
