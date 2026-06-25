# 🏡 End-to-End House Price Prediction Pipeline

An enterprise-grade, containerized machine learning pipeline that predicts residential real estate valuations using an optimized **XGBoost Parallel Random Forest** architecture. The training workflow features a systematic approach to hyperparameter regularizations, dropping an extreme validation-overfitting gap from 27% down to a stable 17%.

## 🚀 Project Highlights
* **Core Architecture**: XGBoost Regressor modified into a Parallel Random Forest ensemble to tame variance.
* **Tuning Optimization**: Optimized via Scikit-Learn's `RandomizedSearchCV` across a constrained architectural search space.

## 📊 Tuning & Validation Journey

During development, standard boosting trees violently overfitted on spatial and variance noise within the housing dataset. Below is the systematic approach taken to stabilize the framework:

| Phase | Search Strategy | Space Constraints | Train R^2 | Test R^2 | Overfitting Gap |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **Baseline** | Standard Boosting | Default Bounds | 0.909 | 0.632 | 27.7% (Extreme) |
| **Pruned** | Extreme Regularization | Max Depth: 2, Lambda: 200 | -0.027 | -0.068 | Broken Math |
| **Optimized** | Parallel Bagging Forest | Max Depth: 4, Parallel Trees: 15 | **0.813** | **0.636** | **17.7% (Stable)** |

> **Key Takeaway**: Switching from sequential boosting to an explicit parallel forest architecture (`num_parallel_tree=15`) with a lowered `max_depth` smoothed out volatile price nodes and successfully broke the test performance ceiling.
