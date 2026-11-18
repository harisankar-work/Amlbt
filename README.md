# AMLBT — Advanced Machine Learning for Business Transformation

Course notes, experiments, and Google Colab notebooks for **Advanced Machine Learning for Business Transformation (AMLBT)**.

> **Repository status:** Initial course README. The topics below are a learning outline based on work discussed in class; notebooks, results, and Colab links have not yet been uploaded or verified.

## Topics and practical work

### 1. Exploratory Data Analysis (EDA)
- Inspect dataset shape, columns, types, missing values, duplicates, and descriptive statistics.
- Explore numerical distributions, categorical variables, outliers, and correlations.
- Visualize relationships between features and the target variable.
- Split data into training and test sets and prevent data leakage.

### 2. Regression models
- **Ordinary Least Squares (OLS) / Linear Regression:** baseline linear relationship.
- **Ridge:** L2 regularization to reduce coefficient magnitude.
- **Lasso:** L1 regularization, which can set some coefficients to zero.
- **Elastic Net:** combines L1 and L2 penalties.
- **Support Vector Regression (SVR):** margin-based nonlinear or linear regression.
- **Decision Tree / Random Forest:** tree-based prediction and bagging.
- **Gradient Boosting / XGBoost:** sequential trees correcting residual errors.
- **Gradient descent:** iterative optimization of model parameters; compare with closed-form OLS.

### 3. Artificial Neural Networks (ANN)
- Dense layers, neurons, weights, biases, and activation functions (including ReLU and sigmoid).
- TensorFlow / Keras model construction.
- Epochs, batches, learning rate, optimizer, loss functions, and hyperparameters.
- Training curves, validation performance, and overfitting.

### 4. Model evaluation and comparison
- Compare models on the **same held-out test set**.
- Metrics: MSE, RMSE, MAE, and R².
- Visualize model comparison and predicted-vs-actual values.
- Tune hyperparameters using validation data or cross-validation, not the test set.
- **Important:** Do not alter results to force an ANN or any other model to achieve the lowest MSE.

## Example case: Bengaluru house-price prediction

A possible regression exercise uses a Bengaluru housing dataset to predict prices from property features. The exact dataset schema, preprocessing steps, model results, and first XGBoost weak learner will be documented after the notebook is added.

## Running notebooks in Google Colab

1. Open a notebook from this repository in [Google Colab](https://colab.research.google.com/).
2. Upload or mount the required dataset, and update its path.
3. Run cells in order, recording package versions and random seeds for reproducibility.
4. Review outputs and evaluation metrics before reporting conclusions.

## Suggested repository structure

```text
Amlbt/
├── README.md
├── notebooks/       # Google Colab .ipynb files
├── data/            # Dataset instructions or small shareable samples
└── results/         # Exported figures and comparison tables
```

## Notebook index

| Notebook | Colab link | Status |
| --- | --- | --- |
| EDA and regression comparison | To be added | Not uploaded |
| TensorFlow ANN | To be added | Not uploaded |

## Notes on reproducibility

Notebook-specific assumptions, dataset provenance, preprocessing, hyperparameters, model architectures, and measured results should be recorded alongside each experiment. No performance numbers are asserted in this README without a corresponding reproducible run.
