# Wine Quality Prediction
## Overview
This notebook applies machine learning techniques to predict the quality of red wine based on various physicochemical properties. The dataset is sourced from the UCI Machine Learning Repository. Three classification models were tested: Logistic Regression, Decision Tree, and Random Forest. Model performance was evaluated using accuracy, precision, recall, and F1-score.

### Dataset
Source: UCI Machine Learning Repository
Description: Dataset contains 1599 instances of red wine samples with 11 features and a quality rating (3–8).
Features:
- fixed acidity, volatile acidity, citric acid, residual sugar, chlorides
- free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol
Target: quality (wine quality score)

### Data Exploration and Preprocessing
Dataset was explored visually using histograms, boxplots, and pair plots.
Strong correlations observed between alcohol, sulphates, and wine quality.
Skewed features were transformed using PowerTransformer() for normalization.
Stratified sampling was applied to maintain the distribution of wine quality scores across train/test sets.

### Modeling
Models trained and evaluated:
1. SVM Regressor:
- MSE:0.29
- RMSE:0.54
- MAE:0.37

2. Fine-tuned SVM Regressor:
- Best parameters by GridSearchCV: 'svm__C': 0.5, 'svm__gamma': 'scale', 'svm__kernel': 'rbf'
- Best parameters by RandomizedSearchCV: 'svm__C': 0.3, 'svm__gamma': 'auto', 'svm__kernel': 'rbf'
- RMSE: 0.63
- MAE: 0.46
- R2: 0.36

### Experimenting
- Implement 'SelectFromModel' transformer in full pipeline
- Implementing StandardScalerClone from scratch

## Acknowledgements
Dataset was provided by the UCI Machine Learning Repository and published on Kaggle.

- Zhan Kazikhanov (Astana IT University)
- jkazikhanov@gmail.com
- https://github.com/don-juann
