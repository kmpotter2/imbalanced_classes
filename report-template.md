# Module 12 Report Template

## Overview of the Analysis

* The purpose of the analysis is to identify the creditworthiness of borrowers.
* The data provided has information identifying loan information for potential borrowers, for which I needed to predict if they were healthy loans or high-risk loans.
* From the provided information I am trying to predict: `confusion_matrix`, `balanced_accuracy_score`, and `classification_report_imbalanced`.
* I had to first model the data, fit the data and finally predict using the data.
* I used `LogisticRegression` and oversampling methods to generate the best predition possible.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Accuracy: Measures how often the model was correct by calculating the ratio of the number of correct predictions to the total number of outcomes.
Precision: Measures how confident we are that the model correctly made the positive predictions by dividing the number of true positive predictions by the number of all positive predictions.
Recall: Measures the number of actually fraudulent transactions that the model correctly classified as fraudulent by dividing the true positive predictions by the true positive predictions plus the false negative predictions.

* Machine Learning Model 1:
  * Orriginal Data Set
  * 0 = healthy loan
  * 1 =  high-risk loan
  * Accuracy: 95%
  * Precision: 0: 100% 1: 85%
  * Recall:  0: 99% 1: 91%

* Machine Learning Model 2:
  * Oversampled Data Set
  * 0 = healthy loan
  * 1 =  high-risk loan
  * Accuracy: 99%
  * Precision: 0: 100% 1: 84%
  * Recall:  0: 99% 1: 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any.
* The precision value for the high-risk loan went down using the oversampled data. However, the accuracy, recall and f1 value went up for the high-risk loan data. Overall, the logistic regression model, fit with oversampled data did a better job at predicting the loan status of the test data. Depending on the data you would like to predict, the orriginal data may be more precise at predicting the true outcome, but will be skewed for the 2nd classified data.
