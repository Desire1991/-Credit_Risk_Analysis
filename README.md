# Credit Risk Analysis

## Overview:

In this project, using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier, and EasyEnsembleClassifier, to predict credit risk. Finally, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results:
**Random Over Sampler (Naive Random Oversampling) Model:**

. Accuracy Score: 0.65

. Precision: 0.99

. Recall: 0.56

. F1: 0.71

![ClusterCentroids](https://user-images.githubusercontent.com/74233163/117128156-a87b8680-ad62-11eb-96e9-cc1a9ea96b4a.png)

**SMOTE Oversampling Model:**

. Accuracy Score: 0.65

. Precision: 0.99

. Recall: 0.69

. F1: 0.81

![Smote](https://user-images.githubusercontent.com/74233163/117127827-3a36c400-ad62-11eb-8e0a-493ad33f9d03.png)

## SMOTE

**Cluster Centroids Undersampling Model:**

. Accuracy Score: 0.65

. Precision: 0.99

. Recall: 0.40

. F1: 0.56

![Cluster Centroids Undersampling Model](https://user-images.githubusercontent.com/74233163/117127479-bf6da900-ad61-11eb-8a25-c43b025959fb.png)
. ClusterCentroids

**SMOTEENN (Combination (Over and Under) Sampling) Model:**

. Accuracy Score: 0.54

. Precision: 0.99

. Recall: 0.57

. F1: 0.72

## SMOTEENN

![Smoteen_combination](https://user-images.githubusercontent.com/74233163/117126748-d65fcb80-ad60-11eb-9afd-2d720da41963.png)



**Balanced Random Forest Classifier Model:**

. Accuracy Score: 0.79

. Precision: 0.99

. Recall: 0.88

. F1: 0.93

# BalancedRandomForestClassifier

![Balanced_RandomForestClassifier](https://user-images.githubusercontent.com/74233163/117126146-f93db000-ad5f-11eb-99b3-249d10eff912.png)

. Accuracy Score: 0.93

. Precision: 0.99

. Recall: 0.94

. F1: 0.97

### AdaBoost

![AdaBoost_classifier](https://user-images.githubusercontent.com/74233163/117125618-63a22080-ad5f-11eb-96c0-7e00764a1630.png)

## Summary:

For all the six models, we can see that the Easy Ensemble Classifier model performs better than the others. At 0.93 Accuracy Score, it has the highest score. The next model is the Balanced Random Forest Classifier model with a 0.79 Accuracy Score. Also, these two models have the highest F1 score - weighted average of the Recall and Precision score, at 0.97 and 0.93 scores, respectively.

With all of these high scores in Recall, Accuracy, and F1 scores, I would suggest using the Easy Ensemble Classifier model for the algorithm to predict credit risk for the LendingClub company.

