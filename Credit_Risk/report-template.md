# Module 12 (20) Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

__* Explain the purpose of the analysis.__
<br> <span style = "color: blue">This analysis was to build and evaluate machine learning models for predicting the healthiness of loads based on financial information and asses the performance of different models to find out if the loans are "healthy" or "high-risk".  This would help for deciding whether or not to approve the loans.</span>

__* Explain what financial information the data was on, and what you needed to predict.__
<br> <span style = "color: blue">The data has features of loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt and loan status (healthy = 0, high-risk = 1). These features were used to predict whether the loan was healthy or high risk. </span>


__* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).__
<br> <span style = "color: blue"> Loan status: O for healthy loan and 1 for high-risk.</span>

__* Describe the stages of the machine learning process you went through as part of this analysis.__
<br> <span style = "color: blue"> 1. Read the lending_data.csv file into a Pandas DataFrame.<br>
2. Create label sets (y) and features (X), review the variable sets and split the data into training and testing by using train_test_split. <br>
3. Create a Logistic Regression Model with the original data.<br>
4. Assess the model's performance by crating the confusion matrix and classification report.</span><br>

__* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).__
<br> <span style = "color: blue">The logistical regression model was used as the primary classification algorithm.</span>

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

  __Confusion Matrix:__<br>
 ![Confusion Matrix](/Challenges/Module%2020%20Credit-Risk-Classification%20Challenge/credit-risk-classification/Credit_Risk/confusion_matrix.png)


  __Classification Report:__<br>
  ![Classification Report](/Challenges/Module%2020%20Credit-Risk-Classification%20Challenge/credit-risk-classification/Credit_Risk/classification_report.png)

- Accuracy of this model is 99%
- Precision for healthy loans (`0`) is 100% / for high-risk loans (`1`) is 85%.
- Recall for healthy loans (`0`) is 99% / for high-risk loans (`1`) is 91%.
- F1-Score for healthy loans (`0`) is 100% / for high-risk loans (`1`) is 88%.



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

**Accuracy** The overall accuracy for the model is 99%.  This indicates that the model correctly predicts the class labels for 99% of the samples in the test dataset. 

**Precision** 
For healthy loans `0`, the model's precision is 100%.  When it predicts a loan as healthy, it is correct every time.   When it predits high-risk loans `1`, the precision is 85% correct, so the predicted high-risk loans are accurate 85% of the time. 

**Recall** 
For healthy loans `0`, the recall is 99%.  This indicates that the model correctly identifies 99% of the actual healthy loans.  For high-risk loans `1`, the model captures 91% of the actual high-risk loans.

**F1-Score** 
For healthly loans `0`, the balance of precision & recall (F1-Score) is 100%  and 88% for high-risk loans `1`.  This is a pretty good balance between precision and recall for both.

The logistic regression model shows a good predictive model for both healthy & high-risk loans.