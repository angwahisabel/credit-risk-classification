# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* **Purpose of the Analysis:**
The purpose of this analysis was to evaluate machine learning models for predicting loan statuses based on various financial features. The goal was to build a model that accurately predicts whether a loan is high-risk or healthy based on the input features.

* Explain what financial information the data was on, and what you needed to predict.
* **Data Description:**

The data provided financial information on loans, where each loan was labeled as either:
  `0` (Healthy Loan): Indicates a loan with a low risk.
  `1` (High-Risk Loan): Indicates a loan with a high risk

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* **Variables to Predict:**
The primary variable of interest to predict was the `loan_status` label, which was binary: `0` or `1`.

* Describe the stages of the machine learning process you went through as part of this analysis.
* **Stages of the Machine Learning Process:**
  1. **Data Preparation:**
  *Loaded and reviewed the dataset.
  *Separated the data into features (`X`) and labels (`y`).
  *Split the data into training and testing sets using `train_test_split`.
  2. **Model Building:**
  *Used the `LogisticRegression` algorithm to create a classification model.
  *Fitted the model using the training data.
  3. **Model Evaluation:**
  *Made predictions using the testing data.
  *Generated a confusion matrix to assess model performance.
  *Printed a classification report to evaluate precision, recall, and F1-scores.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
* **Methods Used:**
  **Logistic Regression**: A classification algorithm used to predict the probability of a categorical dependent variable. In this analysis, it was used to predict the likelihood of a loan being high-risk (`1`) or healthy (`0`).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
* Description of Model 1 Accuracy, Precision, and Recall scores.
* **Machine Learning Model 1: Logistic Regression**
**Accuracy**: 99% (overall accuracy of predictions)
  **Precision**:
  *Healthy Loan (`0`): 1.00
  *High-Risk Loan (`1`): 0.85
**Recall**:
  *Healthy Loan (`0`): 0.99
  *High-Risk Loan (`1`): 0.91
**F1-score**:
  *Healthy Loan (`0`): 1.00
  *High-Risk Loan (`1`): 0.88

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
**Model Performance:**
  The Logistic Regression model performs exceptionally well, with high accuracy and strong metrics for predicting `0` (Healthy Loans). It has slightly lower precision and recall for `1` (High-Risk Loans), but still performs well in identifying high-risk loans.

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
* **Recommendation:**
  **Best Performing Model:** The Logistic Regression model appears to be the best-performing model based on the evaluation metrics. It shows excellent precision and recall for predicting healthy loans and good performance for high-risk loans.
  **Importance of Prediction:** In this context, predicting high-risk loans (`1`) might be more critical than predicting healthy loans (`0`). High-risk loans often require more attention and intervention, so a model with good recall for high-risk loans is valuable.

If the current model’s performance on high-risk loans is deemed sufficient, it would be recommended for use. If there is a need to improve recall for high-risk loans further, additional techniques such as hyperparameter tuning or exploring alternative algorithms might be considered.

If you do not recommend any of the models, please justify your reasoning.
