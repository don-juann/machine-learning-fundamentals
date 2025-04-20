# Batch Gradient Descent using NumPy

## Overview
This notebook demonstrates the implementation of a Batch Gradient Descent algorithm using NumPy (without Scikit-Learn, to develop better understanding of BatchGD algorithm) for softmax regression. It trains a multiclass classification model to classify the Iris dataset, which contains measurements of flower characteristics. The project focuses on building a gradient descent model, optimizing it, and evaluating its performance on a test set.

## Key Features
### Retrieving Data:
- Fetching popular Iris dataset from the UCI Machine Learning Repository using the ucimlrepo library.
- Preprocessing the dataset by normalizing X features and one-hot encoding the y target labels.

### Multiclass Classification:
- Implementing softmax regression to classify the Iris dataset into three classes based on the flower species.

### Gradient Descent Optimization:
- Develops the Batch Gradient Descent algorithm to optimize model parameters.
- Utilizes cross-entropy loss as the objective function.
- Implements early stopping to prevent overfitting.

### Testing and Evaluation:
- Tests the model on unseen data.
- Calculates the accuracy of predictions for performance evaluation.

### Dependencies
Ensure the following libraries are installed in your Python environment:
- numpy
- pandas
- scikit-learn
- ucimlrepo

### Results

The model in this notebook achieves a classification accuracy of 100% on the test set for the Iris dataset. The results showcase the effective implementation of Batch Gradient Descent with softmax regression for multiclass classification tasks using NumPy.

### Acknowledgements
Dataset provided by the UCI Machine Learning Repository.
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- https://github.com/don-juann
