# LendingClub Credit Risk Analysis

![credit cards](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/stephen-phillips-hostreviews-co-uk-em37kS8WJJQ-unsplash.jpg)

## Overview of Analysis

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then I used a combinatorial approach of over-and-undersampling using the SMOTEENN algorithm. I then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

### Deliverable 1 
Used the oversampling RandomOverSampler and SMOTE algorithms, and then used the undersampling ClusterCentroids algorithm. Using these algorithms, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

Here are the classification reports from reach to compare:

  - RandomOverSampler

  ![RandomOverSampler](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/RandomOverSample.png)
  
  - SMOTE

  ![SMOTE Oversample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/SMOTEResample.png)

  - ClusterCentroids

  ![ClusterCentroids Resample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/ClusterCentroidsResample.png)

### Deliverable 2 
Used a combinatorial approach of over-and-ndersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, I resampled the dataset, viewed the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

SMOTEENN Classification report:

  ![SMOTEENN Resample](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/SMOTTEENResample.png)

### Deliverable 3 
Trained and compared two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. Using both algorithms, I resampled the dataset, viewed the count of the target classes, trained the ensemble classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

Here are the classification reports from both to compare

  - BalancedRandomForestClassifier

  ![BalancedRandomForestClassifier](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/BalancedRFClassifier.png)

  - EasyEnsembleClassifier

  ![EasyEnsembleClassifier](https://github.com/RyanWhited/Credit_Risk_Analysis/blob/main/images/EasyEnsembleClassifier.png)
