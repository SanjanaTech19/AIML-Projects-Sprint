# Wine Quality Prediction

This project predicts the quality of red wine using a Random Forest classifier.
The notebook loads the `wineQualityReds.csv` dataset, performs basic exploratory data analysis, preprocesses the data, trains a model, evaluates accuracy, and builds a sample prediction system.

## Files

- `wine-quality.ipynb` - Jupyter notebook containing the full analysis and model pipeline.
- `wineQualityReds.csv` - red wine dataset used for training and evaluation.
- `requirements.txt` - Python package dependencies.
- `.gitignore` - files and folders to exclude from Git.

## Setup

1. Create and activate a Python virtual environment:

```bash
python -m venv venv
venv\Scripts\activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open `wine-quality.ipynb` in Jupyter Notebook or VS Code and run the cells.

## Notes

- The notebook uses `pandas` for data loading and preprocessing.
- Seaborn and Matplotlib are used for visualization.
- `RandomForestClassifier` from scikit-learn is used to train and evaluate the model.
- The notebook includes a sample prediction step for a single wine record.

## Usage

Run the notebook, then update the `input_data` tuple in the prediction section to test new wines.
