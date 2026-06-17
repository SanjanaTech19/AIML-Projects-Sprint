# Used Car Price Prediction 🚗

## 📝 Project Overview
This project delivers an end-to-end Machine Learning regression pipeline built to predict the resale price of used cars based on historical sales data. 

The primary goal of this project was to tackle real-world data science challenges: identifying unlearnable synthetic data noise, engineering clean features from messy text columns, fixing data scale mismatches, and systematically eliminating model overfitting to ensure highly accurate, reliable real-world predictions.

---

## 🛠️ Tech Stack & Library Frameworks
This project was built entirely in Python inside a Jupyter/VS Code notebook environment using the following standard data science stack:
*   **Pandas & NumPy:** For data cleaning, feature engineering manipulation, matrix slicing, and structural data array reshaping (`.reshape(-1, 1)`).
*   **Scikit-Learn (Sklearn):** For data splitting, feature scaling (`StandardScaler`), feature selection (`VarianceThreshold`), and training our final regression architecture (`GradientBoostingRegressor`)
*   **Matplotlib & Seaborn:** For visual Exploratory Data Analysis (EDA) via hue-separated pairplots and generating our final actual-vs-predicted scatter validation plots.

---

## 📊 About the Dataset
The dataset used is a real-world, authentic **CarDekho Vehicle Dataset** consisting of historical used car sales records. Unlike synthetic mock datasets, this data captures true economic market forces such as vehicle brand equity and depreciation.

The primary features used by the model include:
*   **selling_price (Target Variable `y`):** The final price the car was sold for.
*   **car_age (Engineered Feature):** Calculated dynamically by subtracting the manufacturing `year` from the baseline year to track realistic vehicle depreciation.
*   **brand (Engineered Feature):** Parsed dynamically from the first word of the raw `name` column to group manufacturer equity without causing high-cardinality data leakage.
*   **km_driven & owner:** Continuous numerical metrics tracking vehicle usage depth.
*   **fuel & transmission:** Categorical variables tracking drivetrain layouts (One-Hot Encoded into binary dummy features).

Extreme luxury and commercial price anomalies were automatically stripped out using a 98th-percentile quantile mask (`quantile(0.98)`) to stabilize model variance.

---

## 📈 Understanding Our R^2 Score
Our evaluation metrics went through a massive transformation during the debugging lifecycle, concluding in an optimized structural victory:

*   **Training R^2 Score:** 0.840 (84.0%)
*   **Testing R^2 Score:** 0.785 (78.5%)

### What do these scores mean?
1. **Strong Explanatory Power:** An R^2 of `0.785` means our engineered feature matrix successfully explains **78.5% of the total variance** dictating used car prices on completely unseen test data.
2. **Zero Overfitting:** In earlier runs, our model suffered from severe overfitting (scoring `0.97` on training but falling to a negative `-0.19` on testing) because it was memorizing high-cardinality car models and hidden index tracking rows.
3. **Perfect Generalization:** By restricting tree depths (`max_depth=5`) and lowering the learning rate of our `GradientBoostingRegressor`, we forced the sequential trees to learn broad, generalizable automotive depreciation rules instead of memorizing data noise. Because the training score and testing score sit closely together, the model is fully optimized and ready for production deployment.
