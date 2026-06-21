Big Mart Sales Prediction

A machine learning project designed to forecast product sales at retail outlets. By modeling sales patterns across various item categories and store types, this system helps inventory managers optimize supply chains and increase overall store revenue.

About the Project

Predicting retail sales is highly challenging due to shifting consumer behavior, product placements, and store attributes. This project cleans raw transactional data, handles missing attributes via structural data mappings, and applies a regularized gradient-boosting model to predict target sales figures across distinct commercial outlets.

Dataset 

Big Mart Sales Dataset 
Key Features: Item_Identifier, Item_Weight, Item_Fat_Content, Item_Visibility, Item_Type, Item_MRP, Outlet_Identifier, Outlet_Size, Outlet_Esatablishment_Year, Outlet_Location_Type, Outlet_Type, Item_Outlet_sales,
Target Variable: Item_Outlet_Sales

Tools & Libraries Used

Language: Python
Data Manipulation: pandas, numpy
Data Visualization: matplotlib, seaborn
Machine Learning Model: xgboost (XGBRegressor)
Evaluation Metrics: scikit-learn (metrics.r2_score)

Model Performance

The final model was carefully tuned with custom tree depth restrictions and weight regularization to eliminate overfitting, matching top benchmark results for this dataset.

Training R2 Score: 0.645
Test R2 Score: 0.586