# Mutual-Fund-Prediction
Built a TFT-based system to predict returns and suggest optimal portfolios for 80+ mutual funds using data from ETmoney and AMFI, achieving ~8% return on test data.

📊 Mutual Fund Return Prediction & Portfolio Suggestion System
This project aims to build an intelligent system for forecasting mutual fund returns and suggesting an optimal investment portfolio. It leverages the Temporal Fusion Transformer (TFT) — a deep learning model specifically designed for interpretable time series forecasting — to make return predictions based on historical mutual fund data.

🔍 Objective
Predict future returns of mutual funds.

Design an allocation strategy that balances high returns and portfolio stability.

Help users make data-driven investment decisions.

🧠 Approach
Data Collection & Preprocessing

Scraped and cleaned monthly and annual return data of 80+ mutual funds from ETmoney and AMFI.

Combined and standardized data for modeling.

Modeling with TFT

Implemented a Temporal Fusion Transformer (TFT) using TensorFlow/Keras.

Trained the model on cleaned data to forecast one-month-ahead returns.

Portfolio Allocation Logic

Ranked funds based on predicted return and historical stability.

Allocated weights using a hybrid strategy:

20%, 20%, 15%, 15%, 10%, 10%, 5%, 5% based on rank.

Balanced risk and growth by considering both return and volatility.

Performance Evaluation

Backtested the portfolio using historical data.

Achieved ~8% return on test data using the generated portfolio.

📁 Files
Mutual_Fund_Return_Prediction.ipynb: Main notebook for return prediction using TFT.

(Other files like cleaned data, prediction-based allocation, and return calculation logic can be listed here when uploaded.)

📌 Technologies Used
Python, Pandas, NumPy

TensorFlow/Keras

Temporal Fusion Transformer (TFT)

Matplotlib/Seaborn (for visualization)

🚀 Future Work
Extend prediction window (multi-step forecasting).

Integrate real-time data via APIs.

Add risk-adjusted metrics (e.g., Sharpe Ratio) for better allocation.
