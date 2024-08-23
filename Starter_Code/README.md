# Credit Risk Classification

The purpose of this analysis was to evaluate machine learning models for predicting loan statuses based on various financial features. The goal was to build a model that accurately predicts whether a loan is high-risk or healthy based on the input features.

* **Data Description:**

The data provided financial information on loans, where each loan was labeled as either:
  `0` (Healthy Loan): Indicates a loan with a low risk.
  `1` (High-Risk Loan): Indicates a loan with a high risk

* **Variables to Predict:**
The primary variable of interest to predict was the `loan_status` label, which was binary: `0` or `1`

* **Methods Used:**
  **Logistic Regression**: A classification algorithm used to predict the probability of a categorical dependent variable. In this analysis, it was used to predict the likelihood of a loan being high-risk (`1`) or healthy (`0`).

## Results

  The Logistic Regression model performs exceptionally well, with high accuracy and strong metrics for predicting `0` (Healthy Loans). It has slightly lower precision and recall for `1` (High-Risk Loans), but still performs well in identifying high-risk loans.
