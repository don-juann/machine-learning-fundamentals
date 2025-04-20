# MNIST Classification
## Overview
This notebook is used  for exploratory learning and building machine learning models for the MNIST dataset, which is a collection of handwritten digit images, typically used for classification tasks. The notebook covers various machine learning techniques and evaluates performance of models.

### Dependencies
Following libraries were used:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

### Retrieving Data:
- Load and preprocess the MNIST dataset.

### Multiclass Classification:
Implementing a multiclass classification model to distinguish between digits (0-9).

### Multioutput Classification (Cleaning Noise):
- Perform classification tasks while handling noisy data.
- Introduce techniques for cleaning and improving the dataset quality.

### Building Accurate Model using KNeighborsClassifier:
Experimenting with different architectures and hyperparameters to optimize model performance:
- Best parameters: n_neightbors = 3, weights = 'distance'
- Accuracy score: 0.972
- F1: 0.972

### Manually Creating Augmented Images:
- Manually benerating new training data using Numpy to improve generalization.

### Binary Classifiers:
Stochastic Gradient Descent Classifier for binary classification:
- TrueNegative = 53892 (Correctly classified as non-5)
- FalsePositive = 687 (Incorrectly classified as 5)
- FalseNegative = 1891 (Incorrectly classified as non-5)
- TruePositive = 3530 (Correctly classified as 5)
- roc_auc_score = 0.96

Random Forest Classifier for binary classification:
- f1: 0.9274509803921569
- roc_auc_score: 0.9358174809192218

## Acknowledgements
Dataset was provided by the UCI Machine Learning Repository and published on Kaggle.
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- github.com/don-juann
