Tesla Next-Day Stock Price Forecasting

 Project Overview

I created this project to see if machine learning could help make short-term predictions for Tesla (TSLA) stock prices.

I used past market data to build an XGBoost regression model that predicts the next day's percentage return, then turned that into an estimated closing price.

I focused not only on building a model, but also on using a realistic time-series process with good validation, feature engineering, and comparing to benchmarks.

Concepts Used

Python | Pandas | NumPy | Matplotlib | Scikit-learn | XGBoost | GridSearchCV | TimeSeriesSplit

What I Did

- Cleaned and validated historical Tesla market data.
- Engineered lagged returns, momentum, volatility, moving-average and volume-based features.
- Used a chronological train/test split to prevent future-data leakage.
- Tuned XGBoost using time-series cross-validation.
- Compared the model against a simple previous-close baseline.
- Evaluated performance using MAE, RMSE and directional accuracy.

Model Performance

My XGBoost model achieved approximately:

- MAE: $14.23
- RMSE: $20.40
- Directional Accuracy: 53.5%

The MAE shows that, on average, my predicted next-day closing price was about $14 off from the real value.

The RMSE is higher because it puts more emphasis on bigger prediction mistakes.

Main Modeling Lesson

The biggest lesson I learned from this project is that a more complex machine learning model does not always outperform a simple baseline.

Even though I used feature engineering, XGBoost, and tuned the model, the final results were very close to just using the previous closing price to predict the next day.

This reinforced the importance of:

- comparing models against meaningful baselines;
- preventing data leakage;
- using time-aware validation;
- evaluating models with appropriate metrics;
- interpreting results critically rather than focusing only on model complexity.

For me, this was one of the most valuable parts of the project because it showed that good data science is not about making a model look successful. It's about really understanding what the results mean.

Skills Demonstrated

Time-Series Analysis | Feature Engineering | XGBoost | Financial Data Analysis | Model Evaluation | Hyperparameter Tuning | Data Leakage Prevention | Critical Model Interpretation

