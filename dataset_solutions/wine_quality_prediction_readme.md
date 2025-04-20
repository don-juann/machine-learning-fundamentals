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
Three models were trained and evaluated:
1. Logistic Regression
Accuracy: 0.69
Precision: 0.56
Recall: 0.52
F1-score: 0.53

2. Decision Tree
Best Parameters: max_depth=10, min_samples_split=5
Accuracy: 0.74
Precision: 0.63
Recall: 0.60
F1-score: 0.61

3. Random Forest
Best Parameters: n_estimators=100, max_depth=12, min_samples_split=5
Accuracy: 0.81
Precision: 0.71
Recall: 0.70
F1-score: 0.70

### Evaluation and Insights
Random Forest outperformed both Logistic Regression and Decision Tree in all key metrics.
Feature Importance (Top 3):
- Alcohol
- Sulphates
- Volatile Acidity

Alcohol content had the strongest positive correlation with wine quality.

## Acknowledgements
Dataset was provided by the UCI Machine Learning Repository and published on Kaggle.

- Zhan Kazikhanov (Astana IT University)
- jkazikhanov@gmail.com
- https://github.com/don-juann
