# Hospital Readmission Prediction

## Overview

This project predicts whether a patient is likely to be readmitted to the hospital using Machine Learning.

Logistic Regression is used to build the prediction model. The project also compares Logistic Regression **with L2 regularization** and **without regularization**.

## Dataset

The dataset used in this project is:

`hospital_readmissions.csv`

The target column is:

`readmitted`

The target values are converted as:

* `no` → 0
* `yes` → 1

## Methodology

The following steps are performed:

1. Load the dataset
2. Check and preprocess the data
3. Encode categorical columns using Label Encoding
4. Separate features and target variable
5. Split the data into training and testing sets
6. Scale the features using StandardScaler
7. Train Logistic Regression with L2 regularization
8. Train Logistic Regression without regularization
9. Compare the two models
10. Evaluate the models using different metrics

## Models Used

### 1. Logistic Regression with L2 Regularization

L2 regularization is used to reduce the effect of large model coefficients and help control overfitting.

### 2. Logistic Regression without Regularization

A Logistic Regression model is also trained without regularization for comparison.

## Evaluation Metrics

The models are compared using:

* Accuracy
* Precision
* Recall
* ROC-AUC
* Confusion Matrix
* ROC Curve

## Clinical Cost

False Negatives are considered important in this case.

A **False Negative** occurs when:

> The patient is actually readmitted, but the model predicts that the patient will not be readmitted.

A False Negative may be important because a high-risk patient may not receive additional monitoring or follow-up.

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

## Files

* `Hospital_Readmission.ipynb` — Jupyter/Google Colab notebook containing the complete implementation.
* `hospital_readmissions.csv` — Dataset used for the project.

## Conclusion

This project demonstrates how Logistic Regression can be used for hospital readmission prediction and how model performance can be compared with and without L2 regularization.


