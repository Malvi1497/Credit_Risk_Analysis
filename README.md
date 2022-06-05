# Credit_Risk_Analysis
## Aim
To evaluate the performance of supervised machine learning models to make a written recommendation on whether they should be used to predict credit risk.
## Overview
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will oversample the data using the RandomOverSampler and SMOTE algorithms, and under sample the data using the ClusterCentroids algorithm. Used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results
* Naive Random Oversampling results: Our balanced accuracy test it 67%, the precision for the high_risk has a very low positivity at 1% and the recall is 74%
naive.
* SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall
smote.
* Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 41%
undersampling.
* Combination(over and undersampling) results: balanced accuracy score is 54.7% the precision is 99% and the recall is 57% overall
combination.
* Balanced Random Forest Classifier results: the accuracy score is 77.2% the precision is 99% and the recall is 88%
random forest.
* Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 94%
ensemble.

## Summary:
In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
