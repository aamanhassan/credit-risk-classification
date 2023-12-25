

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The primary objective of this analysis is to evaluate the accuracy of the linear regression model in predicting healthy loans vs high_risk loans, when applied to both the original and resampled datasets.

* Explain what financial information the data was on, and what you needed to predict.

loan_status is the predictions.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

Original data:
loan_status

0     75036

1     2500

Oversampled:
loan_status

0    56271

1    56271


* Describe the stages of the machine learning process you went through as part of this analysis.

## Stages of Analysis:

1. Prepare Data

2. Separate the data into labels and features.

3. Check the balance of our target values

4. Split the data using train_test_split.

5. Instantiate the Logistic Regression model and fit model with training data.

6. Predict using test data.

7. Calculated the balanced_accuracy score of the model.
   
8. Generate a confusion matrix for the model.
   
9. Print the classification report for the model for orignal data.
    
10. Instantiate the random oversampler model.
    
11. Fit the original training data to the random_oversampler model.
    
12. Count the distinct values of the resampled labels data.
    
13. Instantiate the Logistic Regression model for resampled data.
    
14. Fit the model using the resampled training data.
    
15. Make a prediction using the testing data.
    
16. Calculate the accuracy score of the model.
    
17. Generate a confusion matrix.
    
19. Print the classification report for orignal and resampled data.
    
21. Do the analysis for both data models.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

.sklearn LogisticRegression

.train_test_split

.confusion_matrix

.balanced_accuracy_score

.classification_report

.RandomOverSampler


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  *Description of Model 1 
  *Accuracy 0.99,
  *Precision class 0: 1.00
             class 1: 0.85
  *Recall scores class 0: 0.99
                 class 1: 0.91
    


* Machine Learning Model 2:
  * Description of Model 2 
  * Accuracy 0.99 , 
  * Precision class 0: 1.00
              class 1: 0.84
  * Recall scores class 0: 0.99
                  class 1: 0.99



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
* to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
If you do not recommend any of the models, please justify your reasoning.

In summary, the logistic regression model demonstrates strong overall performance, particularly excelling in predicting class 0 (Healthy Loan). The precision and recall scores for this class are exceptionally high, indicating a robust ability to correctly identify healthy loans without many false positives or negatives.

For class 1 (High-Risk Loan), the precision level is 0.84, and the recall is 0.91. This suggests that the model is more prone to false positives than false negatives, indicating a tendency to predict high-risk loans when they might not be as prevalent.

Considering these results, the logistic regression model appears to be well-suited for predicting both healthy loans and high-risk loans. 

Although logistic regression looks promising in predicting healthy loan status, it is crucial to assess its performance with different datasets to confirm its suitability for predicting the status of healthy loans.


