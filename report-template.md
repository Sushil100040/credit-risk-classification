# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:


The goal of the analysis was to use machine learning to build a model that can identify the credit risk of borrowers based on historical lending  data. Logistic Regression algorithm was chosen as it is widely used for classification problems. The model generated a high accuracy score of 95%, but its recall value for non-healthy loans was lower than for healthy loans, indicating that it is better at predicting healthy loans. This is due to the imbalanced dataset, with healthy loans being much more prevalent.

A Logistic Regression Model was developed using the lending company's dataset, which achieved a 95% accuracy score. However, the model's recall value for non-healthy loans (0.91) was lower than for healthy loans (0.99), indicating a better ability to predict healthy loans. This is due to an imbalanced dataset, with healthy loans being significantly more prevalent than non-healthy loans.

In step 3,(Split the data into training and testing sets) the code was examined, and the value_counts function was used to determine that the dataset is significantly imbalanced, with healthy loans (0) being the majority class and non-healthy loans (1) being the minority class. The confusion matrix in the same step showed that out of 18,765 healthy loans, the model correctly predicted 18,663, and incorrectly predicted 102. For non-healthy loans, out of 619, the model correctly predicted 563 and incorrectly predicted 56.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Logistic Regression Model fitted with Imbalanced Data 
Accuracy Score: 0.95
Healthy loans (Class 0): Precision: 1.00 Recall: 0.99
High-risk loans (Class 1): Precision: 0.85 Recall: 0.91

Machine Learning Model 2:
Logistic Regression Model fitted with Balanced (oversampled) Data
Accuracy, Precision, and Recall scores.
Balanced Accuracy Score: 0.99
Healthy loans (Class 0): Precision: 1.00 Recall: 0.99
High-risk loans (Class 1): Precision: 0.84 Recall: 0.99

## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Model fitted with Imbalanced Data:
56 (FALSE POSITIVES) ----- The actual value is healthy and the predicted value is non-healthy
102 (FALSE NEGATIVES) ----- The actual value is non-healthy and the predicted value is healthy

Model fitted with Balanced Data:
4 (FALSE POSITIVES) --> The actual value is healthy and the predicted value is non-healthy
116 (FALSE NEGATIVES) --> The actual value is non-healthy and the predicted value is healthy

In order to minimize losses, a lending company would prioritize a model that correctly classifies healthy loans and non-healthy loans. Misclassifying healthy loans as non-healthy can result in a loss of customers, while misclassifying non-healthy loans as healthy can result in a loss of funds. The Logistic Regression model fitted with OverSampled data performed better than the model fitted with Imbalanced data, as it resulted in a higher accuracy score and recall. The lending company would prefer fewer False Positives to avoid misclassifying non-healthy loans as healthy, which could result in the loss of provided funds. The confusion matrices showed that the number of False Positives drastically decreased with the balanced data model, indicating a better ability to classify healthy and non-healthy loans correctly. Therefore, it is recommended to use the Logistic Regression Model fitted with Balanced (oversampled) data.
 It is more important to predict the 1's, because we want to know the high risk loans, so 1's is better

