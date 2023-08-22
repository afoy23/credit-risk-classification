# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this analysis is to evaluate the performance of two logistic regression machine learning models in predicting the credit risk associated with loans.

* Explain what financial information the data was on, and what you needed to predict.

The analysis was conducted on financial data of loan sizes, interest rates, borrowers income, debt-to-income ratios, number of accounts, derogatory marks, and total debt.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The objective was to predict the loan status, being either a healthy loan of ('0') or high-risk loan of ('1').

* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

1. Load data
2. Create the labels and features
3. Check the balance using value_counts
4. Split the datasets for training and testing sets
5. Create and fit a logistic regression model with data
6. Predict the data
7. Evaluate the model's performance by observing accuracy, precision, recall, and f1 scores
8. Resample the data with RandomOverSampler
9. Create and fit a secondary logistic regression model with resampled data
10.Evaluate the secondary model's performance by observing the same accuracy, precision, recall, and f1 scores

## Results

* Machine Learning Model 1:
  * Accuracy: 99%
   
  * Precision:  
    * Healthy Loans ('O') - 1.00
    * High-Risk Loans ('1') - 0.89
  * Recall:  
    * Healthy Loans ('O') - 1.00
    * High-Risk Loans ('1') - 0.87
  

* Machine Learning Model 2:
  * Accuracy: 100%
   
  * Precision:  
    * Healthy Loans ('O') - 1.00
    * High-Risk Loans ('1') - 0.87
  * Recall:  
    * Healthy Loans ('O') - 1.00
    * High-Risk Loans ('1') - 1.00

## Summary

Both models perform very strongly when predicting healthy loans. With the second model, using the resampled data, accuracy and recall greatly improved to nearly perfect scores. Precision remains an issue with both models, staying at 87%.  
The recommendation is to use Model 2.  
Since both models correctly predict healthy loans, it is more prudent to have a model that correctly classifies more high-risk loans, even. The risk associated with misclassifying a healthy loan as high-risk is lower than the risk of not classifying a high-risk loan as such.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

I recommend model 2 using logistic regression the accuracy has improved compared to model 1. 
