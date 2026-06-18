# Loan Status Prediction using SVM

This project builds a predictive machine learning model to automate loan eligibility screening. By analyzing customer details provided during online applications, the system determines whether a loan application should be approved or rejected.

## 📊 Dataset

* **Source:** Kaggle
* **Description:** Historical records containing applicant demographics, financial status, and prior credit histories.
* **Target Variable:** `Loan_Status` (1 = Approved, 0 = Rejected)
* **Key Features:**
  * Gender, Marital Status, Dependents, Education, Self-Employment
  * Applicant & Co-applicant Income
  * Loan Amount & Loan Amount Term
  * Credit History, Property Area

## 🛠️ Tools & Technologies Used

* **Language:** Python
* **Data Manipulation & Preprocessing:** Pandas, NumPy, StandardScaler
* **Data Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (Support Vector Machine Classifier)
* **Development Environment:** VS Code / Jupyter Notebook

## 📈 Model Performance & Accuracy

The **Support Vector Classifier (SVC)** was evaluated using standard classification metrics on a held-out test dataset of 48 samples.

* **Training Accuracy:** **80.56%**
* **Test Accuracy:** **83.33%**

### Detailed Classification Report (Test Data)

| Class (Status) | Precision | Recall | F1-Score | Support |
| :--- | :---: | :---: | :---: | :---: |
| **0 (Rejected)** | 0.82 | 0.60 | 0.69 | 15 |
| **1 (Approved)** | 0.84 | 0.94 | 0.89 | 33 |
| **Macro Average** | 0.83 | 0.77 | 0.79 | 48 |
| **Weighted Average** | 0.83 | 0.83 | 0.83 | 48 |

## 🚀 How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas numpy scikit-learn seaborn matplotlib
   ```
3. Run the notebook in VS Code or Jupyter:
   ```bash
   jupyter notebook loan_prediction.ipynb
   ```
