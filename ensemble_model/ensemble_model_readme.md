# Practical application of Ensemble models
## Overview
This notebook showcases the practical use of VotingClassifier and StackingClassifier, including their manually created versions.

### Single Classifiers VS Ensemble classifier
Individual Classifiers:
- RandomForest accuracy: 0.9732
- Extra-Trees accuracy: 0.9743
- Support Vector Machine accuracy: 0.9802

Ensemble Classifiers:
- Hard voting accuracy: 0.9772
- Soft voting accuracy: 0.9803

As a result, soft voting classifier shows the best performance, with very slight margin between SVM, which is a second place.

### Blender
Manually created blender validation accuracy: 0.9751
Sklearn blender validation accuracy: 0.9818

As a result, native StackingClassifier shows better performance as it is more.

## Ackknowledgements
MNIST dataset provided by sklearn.datasets
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- github.com/don-juann
