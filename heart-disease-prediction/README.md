# Heart Disease Prediction using Logistic Regression

This project aims to predict the presence of heart disease in patients based on various clinical parameters using a **Logistic Regression** model. The project involves data preprocessing, exploratory data analysis, and model building to achieve a reliable predictive system.

## Overview
Heart disease is one of the leading causes of death globally. Early detection and prediction can significantly help in medical intervention. This project utilizes machine learning, specifically Logistic Regression, to classify whether a person has a "Healthy Heart" or a "Defective Heart" based on health metrics.

## Dataset
The dataset used in this project is `heart.csv`, which contains information on 1025 patients.

## Features
The dataset includes the following clinical features:
1. **age**: Age of the patient
2. **sex**: Sex (1 = male; 0 = female)
3. **cp**: Chest pain type (4 values)
4. **trestbps**: Resting blood pressure
5. **chol**: Serum cholesterol in mg/dl
6. **fbs**: Fasting blood sugar > 120 mg/dl
7. **restecg**: Resting electrocardiographic results (values 0,1,2)
8. **thalach**: Maximum heart rate achieved
9. **exang**: Exercise induced angina
10. **oldpeak**: ST depression induced by exercise relative to rest
11. **slope**: The slope of the peak exercise ST segment
12. **ca**: Number of major vessels (0-3) colored by flourosopy
13. **thal**: 0 = normal; 1 = fixed defect; 2 = reversable defect
14. **target**: 1 = Heart Disease, 0 = Healthy Heart

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-disease-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd heart-disease-prediction
   ```
3. Install the required dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

## Usage
1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook heart-disease.ipynb
   ```
2. Run the cells sequentially to see the data processing, model training, and evaluation.
3. You can also use the predictive system block at the end of the notebook to test with new input data.

## Model Performance
The Logistic Regression model was evaluated on a test set (20% of the data) and achieved the following result:
- **Test Accuracy**: ~80.5%

## Technologies Used
- **Python** (v3.11+)
- **Pandas** & **NumPy** for data manipulation
- **Matplotlib** & **Seaborn** for data visualization
- **Scikit-learn** for machine learning and evaluation
