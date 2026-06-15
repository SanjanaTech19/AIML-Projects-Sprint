# Diabetes Prediction using Logistic Regression

## 📌 Project Overview
This project focuses on predicting the likelihood of diabetes in patients based on several clinical features. Using a **Logistic Regression** model, we analyze key indicators such as age, BMI, blood glucose levels, and medical history to provide early-stage diagnostic insights.

## 📊 Dataset Details
The dataset (`diabetes_prediction_dataset.csv`) contains the following clinical parameters:
- **Gender**: Male, Female, or Other.
- **Age**: Patient's age.
- **Hypertension**: 0 if not present, 1 if present.
- **Heart Disease**: 0 if not present, 1 if present.
- **Smoking History**: Patient's smoking status (never, current, former, etc.).
- **BMI**: Body Mass Index.
- **HbA1c Level**: Hemoglobin A1c level (average blood sugar over 3 months).
- **Blood Glucose Level**: Current blood sugar level.
- **Diabetes (Target)**: 0 (No Diabetes), 1 (Diabetes).

## 🚀 Key Features
- **Exploratory Data Analysis (EDA)**: Comprehensive data visualization using Seaborn and Matplotlib.
- **Data Preprocessing**: Handling categorical variables through mapping and label encoding.
- **Model Building**: Implementing a classification model using Scikit-Learn's Logistic Regression.
- **Evaluation**: Assessing performance using Accuracy Scores and Classification Reports.

## 🛠️ Requirements
Ensure you have the following installed:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

## 💻 How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd diabetes-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook diabetes-prediction.ipynb
   ```

## 📉 Results
The model achieves high accuracy in predicting diabetic status, specifically focusing on the high correlation between **Blood Glucose Levels**, **HbA1c Levels**, and the target outcome.

---
*Created as part of the AI & ML Projects collection.*
