# Practical application of Decision Trees
## Overview
This notebook shows practical use of Decision Trees for classification on moons dataset.
On top of that, Random Forest classifier is created from scratch using multiple Decision Trees.

## Fine-tuning Decision Tree for moons dataset
- make_moons() used to create dataset of 10000 instances
- Dataset was split into 90/10 for training and testing
- Parameter grid was created to fine-tune a decision tree:
'max_depth': (3, 5, 7),
'max_leaf_nodes': (5, 7, 9),
'criterion': ('gini', 'entropy')
- Best parameters: {'criterion': 'gini', 'max_depth': 3, 'max_leaf_nodes': 5}
- Overall accuracy of decision tree: 0.859

## Random Forest for moons dataset
- The same dataset was used again
- ShuffleSplit was used to create 1000 splits consisting of 100 instances (10000 overall)
- 1000 subsets and 1000 decision trees were created
- Accuracy of a single decision tree: 0.796
- Accuracy of 1000 decision trees (Random Forest): 0.867

## Acknowledgements
Dataset is provided by sklearn.datasets

- Zhan Kazikhanov
- jkazikhanov@gmail.com
- https://github.com/don-juann
