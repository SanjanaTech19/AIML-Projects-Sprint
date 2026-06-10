# Iris Flower Classification

This project trains a K-nearest neighbors classifier on the Iris dataset, tunes hyperparameters with cross-validation, evaluates the model, and saves the final pipeline to `iris_knn_best.joblib`.

## Predict with the saved model

Use `predict.py` to load the saved model and make a prediction on new measurements:

```bash
python predict.py --sepal_length 5.1 --sepal_width 3.5 --petal_length 1.4 --petal_width 0.2
```

The script prints the predicted Iris species and class probabilities.

## Dependencies

Install the dependencies with pip:

```bash
pip install scikit-learn pandas seaborn matplotlib joblib
```
