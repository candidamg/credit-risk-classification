# CREDIT-RISK-CLASSIFICATION
## Module 12 Report

## Overview of the Analysis

The purpose of this analysis is to evaluate a model based on loan risk by using the original and resampled data. We use the data of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. You can have access the data by clicking [here](Credit_Risk/Resources/lending_data.csv).

In order to create the reports the labels were set as (y) being the 'loan_status' and (x) being the remaning columns from the dataset.

For this analysis we need to predict whether the 0 (healthy loan) or the 1 (high-risk loan) labels go well by using the logistic regressing model. The target values used were the loan_status, in this case (y), and the counts are 0: 75036 and 1: 2500. 

When the logistic regression models were created, both for the orignal and the resampled data, the random_state is set to 1. 

To evaluate the model's performance from both the original data and the resampled data the following steps were taken: 

* Calculate the accuracy score of the models; </p>
    In the analysis its noted the balanced accuracy score for the orignal data is 0.95, but with the resampled data the score is 0.99, which is a better result.
* Generate two confusion matrix; and,
* Print the reports.
    The first machine learning model was analyzed with the original data and the second machine learning model with the resampled data.

## Results

* Machine Learning Model 1:
  * accuracy = 0.9520
  * precision = (0) 1.00 & (1) 0.85
  * recall = (0) 0.85 & (1) 0.91

* Machine Learning Model 2:
  * accuracy = 0.9936
  * precision = (0) 1.00 & (1) 0.84
  * recall = (0) 0.99 & (1) 0.99

## Summary

The machine learning model that performed the best was model 2. This is because the accuracy and the recall improved. However, the precision for (1) high-risk loan dropped by 0.01. In my opinion both are equally important to predict as the companies would like to know where the high-risk loan lies and would prefer the model 2 since there was improvement on the accuracy and the recall and not a big difference on the precision value.
