# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to evaluate the performance of various over and under sampling models, along with machine leanring models to reduce bias, in order to provide a written recommendation on whether each model should be used to predict credit risk. We utilized a credit card dataset from LendingClub, a peer-to-peer lending services company.

## Results
1. **RandomOverSampler**
 - balanced accuracy score = 0.65
 - precision
    - high risk = 0.01
    - low risk = 0.99
 - recall
   - high risk = 0.62
   - low risk = 0.68
2. **SMOTE (oversampling)**
 - balanced accuracy score = 0.64
 - precision
    - high risk = 0.01
    - low risk = 1.00
 - recall
   - high risk = 0.63
   - low risk = 0.66
3. **ClusterCentroids (undersampling)**
 - balanced accuracy score = 0.53
 - precision
    - high risk = 0.01
    - low risk = 1.00
 - recall
   - high risk = 0.45
   - low risk = 0.61
 4. **SMOTEENN (over and under)**
 - balanced accuracy score = 0.64
 - precision
    - high risk = 0.01
    - low risk = 1.00
 - recall
   - high risk = 0.70
   - low risk = 0.57
5. **BalancedRandomForestClassifier (ensemble)**
 - balanced accuracy score = 0.91
 - precision
    - high risk = 0.01
    - low risk = 1.00
 - recall
   - high risk = 0.49
   - low risk = 0.63
6. **EasyEnsembleClassifier (ensemble)**
 - balanced accuracy score = 0.94
 - precision
    - high risk = 0.00
    - low risk = 0.99
 - recall
   - high risk = 0.66
   - low risk = 0.31
 
## Summary
All models had an F1 score of 0.01 or 0.02, which means we have a pronounced imbalance between sensitivity and precision. Additionally, none of the models tested had a good precision value for high risk. This does not give us confidence that when high risk is predicted, that it is actually true. This could result in loans not being approved, and potential customers missed. Although the EASYEnsembleClassifier performed the best of the tested models, it did not perform well enough to recommend due to the reasons mentioned above. It performed the best due to a high accuracy value and the best sensitivity for identifying high risk loans.
