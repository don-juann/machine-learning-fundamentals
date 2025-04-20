# Titanic Survival Prediction
## Overview
This notebook applies machine learning models to predict survival outcomes on the Titanic dataset. Several classification models were trained and evaluated, including Logistic Regression, Support Vector Machine, Random Forest, and K-Nearest Neighbors. The project includes feature engineering, preprocessing, hyperparameter tuning, and performance evaluation using various metrics.

### Dataset
Name: Kaggle Titanic - Machine Learning from Disaster
Description: Includes 891 passenger records with features such as age, fare, sex, class, etc.
Features Used: Pclass, Sex, Age, SibSp, Parch, Fare, Embarked
Engineered: Title (from Name), FamilySize, IsAlone
Target: Survived (0 = No, 1 = Yes)

### Data Preprocessing and Feature Engineering
Missing values handled:
- Age: filled with median age by title
- Embarked: filled with mode
Feature encoding: 
- Categorical features encoded with LabelEncoder or one-hot encoding
Created features:
- Title extracted from names
- FamilySize = SibSp + Parch + 1
- IsAlone = 1 if FamilySize == 1

Features were scaled using StandardScaler.

### Modeling
1. Decision Tree Classifier:
- Accuracy: 0.79
- Precision: 0.75
- Recall: 0.76
- F1: 0.75
2. Random Forest Classifier:
- Best parameters: 'criterion': 'gini', 'max_depth': 5, 'n_estimators': 50
- Accuracy: 0.82
- Precision: 0.84
- Recall: 0.69
- F1: 0.76

### Evaluation and Insights
Random Forest achieved the highest overall accuracy and balance between precision and recall.
Performance of the model and results are reasonable, considering the type of dataset we are working with.

## Acknowledgements
Dataset provided by Kaggle.com
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- github.com/don-juann
