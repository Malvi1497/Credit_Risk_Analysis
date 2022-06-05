# Credit_Risk_Analysis
## Aim
To evaluate the performance of supervised machine learning models to make a written recommendation on whether they should be used to predict credit risk.
## Overview
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will oversample the data using the RandomOverSampler and SMOTE algorithms, and under sample the data using the ClusterCentroids algorithm. Used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results
* Naive Random Oversampling results: Our balanced accuracy test it 66%, the precision for the high_risk has a very low positivity at 1% and the recall is 66% naive.

![image](https://user-images.githubusercontent.com/94252681/172032218-7bef236a-637a-4365-bb12-ac30773206c8.png)

* SMOTE oversampling results: the accuracy score is 64%, the precision for the high_risk loans has a low positvity again at 1% and recall is 64% overall smote

![image](https://user-images.githubusercontent.com/94252681/172032232-1d940763-42d0-49a4-8e4b-349ded310615.png)

* Undersampling results: balanced accuracy score is 45% overall, the precision is at 99% and the recall is 45%.

![image](https://user-images.githubusercontent.com/94252681/172032247-e3817742-219f-4d8d-b363-3e0f0a56051a.png)

* Combination(over and undersampling) results: balanced accuracy score is 64% the precision is 99% and the recall is 57% overall combination.

![image](https://user-images.githubusercontent.com/94252681/172032274-bd9a43ae-2e08-4535-865e-b76cd2d44cc3.png)

* Balanced Random Forest Classifier results: the accuracy score is 87.3% the precision is 99% and the recall is 87% random forest.

![image](https://user-images.githubusercontent.com/94252681/172032364-ffe8859d-cb62-4c8f-9e24-41d131e4c317.png)

* Easy Ensemble AdaBoost Classifier results: the accuracy score is 90.0% the precision is 99% and the recall is 90% ensemble.

![image](https://user-images.githubusercontent.com/94252681/172032385-c98462e9-9315-4942-957c-bfca1e9738d5.png)

## Summary:
In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
