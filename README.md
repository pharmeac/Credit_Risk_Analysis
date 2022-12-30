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
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)






