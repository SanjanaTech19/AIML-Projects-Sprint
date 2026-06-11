# Titanic Survival Prediction

This project predicts passenger survival on the Titanic using machine learning classification algorithms.

## Dataset

The dataset contains information about passengers aboard the Titanic, including:
- **PassengerId** - Unique identifier for each passenger
- **Survived** - Target variable (0 = Did not survive, 1 = Survived)
- **Pclass** - Passenger class (1st, 2nd, or 3rd)
- **Name** - Passenger name
- **Sex** - Gender (male/female)
- **Age** - Age in years
- **SibSp** - Number of siblings/spouses aboard
- **Parch** - Number of parents/children aboard
- **Ticket** - Ticket number
- **Fare** - Ticket fare
- **Cabin** - Cabin number
- **Embarked** - Port of embarkation (C, Q, or S)

## Files

- `train.csv` - Training dataset (891 rows)
- `test.csv` - Test dataset
- `titanic-survival.ipynb` - Main Jupyter notebook with full analysis and modeling

## Features

The notebook includes:
- Exploratory Data Analysis (EDA)
- Data preprocessing (handling missing values, encoding categorical features)
- Visualization of survival patterns by passenger attributes
- Model training (Logistic Regression and other classifiers)
- Model evaluation and performance metrics

## Setup

### Prerequisites
- Python 3.7+
- Jupyter Notebook

### Installation

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Launch Jupyter:
```bash
jupyter notebook
```

3. Open `titanic-survival.ipynb` and run cells sequentially.

## Key Preprocessing Steps

1. **Handle Missing Values**
   - Age: Filled with mean value
   - Embarked: Filled with mode (most common value)
   - Cabin: Dropped due to high missing percentage

2. **Encode Categorical Features**
   - Sex: Converted to numeric (male=0, female=1)
   - Embarked: Converted to numeric (S=0, C=1, Q=2)

3. **Data Visualization**
   - Survival counts by sex, class, and embarkation port
   - Distribution of fares and ages

## Results

The trained model provides:
- Accuracy metrics on training and test sets
- Feature importance analysis
- Predictions on unseen data

## License

This project is open source and available under the MIT License.
