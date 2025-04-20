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
1. Logistic Regression
- Accuracy: 0.82
- Precision: 0.78
- Recall: 0.73
- F1-score: 0.75

2. Support Vector Machine (SVM)
- Accuracy: 0.84
- Precision: 0.80
- Recall: 0.76
- F1-score: 0.78

3. Random Forest
- Best Parameters: n_estimators=100, max_depth=8
- Accuracy: 0.86
- Precision: 0.82
- Recall: 0.81
- F1-score: 0.81

4. K-Nearest Neighbors (KNN)
- Best K: 9
- Accuracy: 0.81
- Precision: 0.76
- Recall: 0.75
- F1-score: 0.75

### Evaluation and Insights
Random Forest achieved the highest overall accuracy and balance between precision and recall.
Feature importance highlights: Sex, Title, and Fare were the most impactful predictors.

Engineered features like IsAlone and Title improved model performance.

## Acknowledgements
Dataset provided by Kaggle.com
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- github.com/don-juann
