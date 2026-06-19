Gold Price Prediction using Machine Learning

A machine learning project that utilizes historical market data to forecast gold prices (GLD). 

📌 Project Overview

Predicting financial assets is notoriously difficult due to market noise and high volatility. This project builds an end-to-end predictive pipeline that:Engineered lagged historical pricing features.Implemented a strict chronological chronological time split (80/20 train/test split) to prevent data leakage.Evaluated predictions using a One-Step-Ahead methodology to measure real-world deployment viability.

🛠️ Tools & Technologies Used

Language: Python 3.x
Machine Learning: scikit-learn (Random Forest Regressor)
Data Manipulation: pandas, numpy
Data Visualization: matplotlib. seaborn
Development Environment: VS Code / Jupyter Notebook

📊 The Dataset

The dataset contains historical daily trading records for the Gold Shares ETF (GLD). The core columns utilized during preprocessing include:Date: The chronological timeline of trading days.GLD_Price: The daily closing asset price used as our primary modeling target.Engineered Features:Price_Yesterday (.shift(1)): Previous day closing price.Price_2_Days_Ago (.shift(2)): Closing price from two trading sessions prior.Technical trend components such as rolling windows and moving standard deviations.
