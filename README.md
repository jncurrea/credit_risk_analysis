# Credit Risk Analysis
## Overview
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the goal is to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Lastly, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
### Tools
- Jupyter Notebooks
- SciPy
- SKLearn
- imbalanced-learn

## Results
### Oversampling - Naive Random Oversampling
- Balanced Accuracy Score: 0.65
- Precision Score: 0.01
- Recall Score: 0.63
<img width="716" alt="Screen Shot 2022-04-24 at 11 07 57 PM" src="https://user-images.githubusercontent.com/95834653/165019299-4e46b0c1-5fe0-4310-94c3-f9f3de329dee.png">

### Oversampling - SMOTE
- Balanced Accuracy Score: 0.65
- Precision Score: 0.01
- Recall Score: 0.64
<img width="744" alt="Screen Shot 2022-04-24 at 11 14 52 PM" src="https://user-images.githubusercontent.com/95834653/165019827-43d17eaa-bf07-46f1-b0a4-b9cfd9ea742d.png">

### Undersampling - Cluster Centroids
- Balanced Accuracy Score: 0.50
- Precision Score: 0.01
- Recall Score: 0.59
<img width="717" alt="Screen Shot 2022-04-24 at 11 17 04 PM" src="https://user-images.githubusercontent.com/95834653/165020029-6acccb95-0df6-4a9a-a64d-692042273504.png">

### Combination Sampling - SMOTEENN
- Balanced Accuracy Score: 0.61
- Precision Score: 0.01
- Recall Score: 0.69
<img width="716" alt="Screen Shot 2022-04-24 at 11 18 34 PM" src="https://user-images.githubusercontent.com/95834653/165020174-2ec5527b-805b-4b0c-b9a7-4f945143d622.png">

### Random Forest Classifier
- Balanced Accuracy Score: 0.78
- Precision Score: 0.04
- Recall Score: 0.67
<img width="742" alt="Screen Shot 2022-04-24 at 11 19 19 PM" src="https://user-images.githubusercontent.com/95834653/165020252-008bf60e-c435-4b9d-ac82-8274d57d527a.png">

### AdaBoost Classifier
- Balanced Accuracy Score: 0.93
- Precision Score: 0.07
- Recall Score: 0.91
<img width="729" alt="Screen Shot 2022-04-24 at 11 20 47 PM" src="https://user-images.githubusercontent.com/95834653/165020375-2ee59bdd-b340-49aa-81b5-f33a5e679175.png">

## Summary
- The AdaBoost Classifier has the highest Balanced Accuracy Score out of all of the classifiers and sampling methods tested in this project. This should be the classifier used to predict risk in this challenge. 
- Nonetheless, I would not recommend using any of these classifiers. Even the best one (AdaBoost Classifier) has a low precision for high-risk data points (0.07).




