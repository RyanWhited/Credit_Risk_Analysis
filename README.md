# LendingClub Credit Risk Analysis

![credit cards](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/stephen-phillips-hostreviews-co-uk-em37kS8WJJQ-unsplash.jpg)

## Overview of Analysis

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then I used a combinatorial approach of over-and-undersampling using the SMOTEENN algorithm. I then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

### Deliverable 1 
Used the oversampling RandomOverSampler and SMOTE algorithms, and then used the undersampling ClusterCentroids algorithm. Using these algorithms, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

Here are the balanced accuracy score and classification reports from reach to compare:

  - RandomOverSampler: Accuracy = 0.65

  ![RandomOverSampler](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/RandomOverSample.png)
  
  - SMOTE: Accuracy = 0.62

  ![SMOTE Oversample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/SMOTEResample.png)

  - ClusterCentroids: Accuracy = 0.53

  ![ClusterCentroids Resample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/ClusterCentroidsResample.png)

### Deliverable 2 
Used a combinatorial approach of over-and-ndersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

SMOTEENN: 

  - Accuracy = 0.65
  - Classification report:

  ![SMOTEENN Resample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/SMOTTEENResample.png)

### Deliverable 3 
Trained and compared two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. Using both algorithms, I resampled the dataset, viewed the count of the target classes, trained the ensemble classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

Here are the balanced accuracy scores and classification reports from both to compare

  - BalancedRandomForestClassifier: Accuracy = 0.77

  ![BalancedRandomForestClassifier](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/BalancedRFClassifier.png)

  - EasyEnsembleClassifier: Accuracy = 0.94

  ![EasyEnsembleClassifier](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/EasyEnsembleClassifier.png)
  
  ## Summary
  
All of the resampling models I would not recommended due to their low accuracy score. I assume these models are overfit based on their precisions scores. However, both of the ensemble classifiers performed well and the EasyEnsembleClassifier had the best results with a 94% accuracy score and much better scores all across. 
