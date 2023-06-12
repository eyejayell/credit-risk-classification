# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis was to create a model for predicting whether or not a loan would be healthy or high risk. This factored in the size of the loan, the interest rate, the income of the borrower, their debt-to-income ratio, the number of accoounts, and their total debt. To analyze this data we created two machine learning models - the first one not using resampled data, the second one using resample data. Both models used the LogisticRegression classifier. After running both, we saw that the model using resampled data was significantly more accurate at predicting high-risk loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    * The accuracy of this model is 0.99.
    * The precision of this model for predicting health lones is 1.00, the precision of this model for predicting high-risk loans is 0.87.
    * The recall of this model for healthy loans is 1.0, the recall of this model for high-risk loans is 0.89.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * The accuracy of this model is 0.99.
    * The precision of this model for predicting health lones is 0.99, the precision of this model for predicting high-risk loans is 0.99.
    * The recall of this model for healthy loans is 0.99, the recall of this model for high-risk loans is 0.99.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

Of these two models, the second, resampled model is the better one to use. While it is slightly less succesful in predicting whether or not a loan will be considered healthy, it is significantly better at predicting whether or not the the loan will be considered high-risk. We can see this in both the precision (0.99 for the second model, 0.87 for the first model) and recall (0.99 for the second model, 0.89 for the first). As the goal of this model is to help inform lenders on how best to avoid high-risk loans, a model that is more succesfully able to predict whether or not a loan will end up being high-risk is of greater value to the lender. 

If you do not recommend any of the models, please justify your reasoning.
