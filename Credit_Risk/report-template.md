# Module 12 Credit Risk Report 

## Overview of the Analysis



The purpose of this analysis was to evaluate a model based on loan risk. By using a dataset of historical lending activity from a peer-to-peer lending services company to build a model than can identify creditworthiness of borrowers. The variable we are trying to predict is loan status, which was either a healthy loan or a high risk loan. 

The data in the dataset was split into training and testing sets, and the loan status was isolated as a variable. A losgitics regression model was done using the original data. Then a logistic regression model was done with the resampled training data by using the RandomOverSampler module from the imbalanced-learn libarary to resample the data. It was confirmed that the labels then had an equal number of datapoints. To eveaulate the models performance with both the original data and the resampled data, I calculated the accuracy score of the model, created a confusion matrix, and printed the classification report.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
  precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384




* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
   precision    recall  f1-score   support

           0       0.99      0.99      0.99     56277
           1       0.99      0.99      0.99     56277

    accuracy                           0.99    112554
   macro avg       0.99      0.99      0.99    112554
weighted avg       0.99      0.99      0.99    112554 precision    recall  f1-score   support

Fitted with the oversampled data, the logistic regression model is well better suited to predict the high risk loan label, and the healthy loan label precition is still very high
          
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


 The Machine leanring model 1 does an exceptional job at prediciton the healthy loan '0'. The precision, recall, and f1-score are all 1.00 which is the best it could be. As for the high-risk loan '0' the score are less high but still very good. The model could still imporve closer predictions for the high risk loans.
 
 Fitted with the oversampled data, the Machine Learning Model 2 is well better suited to predict the high risk loan label, and the healthy loan label precition is still very high.
 
 Therefore, I determine that Machine Learning Model 2 is the better model to go with, espcially as it is better at predicting the loans that are high risk loans '1'. This is very important to know for the lending company to protect themselves and reduce financial losses.
