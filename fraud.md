# Predicting Fraudulent Transactions
*ACO 423: Data Science project report*

## Introduction

Fraud is a significant concern for businesses and financial institutions. It occurs when individuals are promised a product or service 
they've paid for but do not receive it, or when someone impersonates another person and conducts unauthorized transactions. To mitigate 
these risks, companies implement fraud prevention models. This project aims to develop an accurate prediction model for fraudulent transactions 
using supervised learning techniques.

## Data Source

Obtaining a suitable dataset for fraud detection is crucial. In this *ACO 423: Data Science project*, a dataset titled 'Fraudulent Transactions Predictions' from 
Kaggle.com was chosen. The data has been generated using PaySim, a financial mobile money simulator designed for fraud 
detection. PaySim simulates mobile money transactions based on real transaction logs while preserving client privacy.

As an illustration, the first few lines of the dataset are given below.

![image](https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/2e32246c-4502-4ba1-a725-a16657fc6c17)


## Data Collection

To collect the data, a Kaggle account was created, and Google Colab was used to upload and store the data in Google Drive. 
A Kaggle account is necessary to access and download the data using a username and key-based authentication method. Once on Google Drive, 
the data was transferred to a local drive, enabling easy access through a Jupyter Notebook file in Visual Studio Code, 
eliminating the need to connect to Kaggle repeatedly.

## Dataset Overview

The dataset consists of a single CSV file named 'Fraud.csv,' with a size of 493.53 MB. It comprises 6,362,620 rows and 11 columns. 
Each row represents a transaction, and the columns include 10 transaction features and a classification label. 
The dataset includes the following features:
- `step`: Represents a unit of time.
- `type`: Indicates the type of transaction.
- `amount`: Denotes the transaction amount in local currency.
- `nameOrig`: Identifies the customer initiating the transaction.
- `oldbalanceOrg`: Represents the initial balance before the transaction.
- `newbalanceOrig`: Indicates the new balance after the transaction.
- `nameDest`: Identifies the recipient customer.
- `oldbalanceDest`: Represents the initial balance for the recipient after the transaction.
- `newbalanceDest`: Indicates the new balance for the recipient after the transaction.
- `isFlaggedFraud`: Flags illegal attempts, such as transferring more than $200,000 in a single transaction.
- `isFraud`: Indicates whether the transaction was fraudulent.

  ![image](https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/3cad919e-ed9d-42d3-803d-a31b6d0a012f)


## Data Preprocessing

Data preprocessing is essential to prepare the data for analysis. Key steps include:
1. Examining transaction types to identify which types have the most fraudulent transactions (`TRANSFER` and `CASH_OUT`).
2. Identifying and removing correlated features (`oldBalanceOrig` and `newBalanceOrig`, `oldBalanceDest` and `newBalanceDest`).
3. Removing redundant non-numerical features (`nameOrig` and `nameDest`).
4. Encoding the `type` feature with numerical values (0-4) to make it suitable for analysis.
5. Ensuring there are no missing or invalid values in the dataset.

![transactionTypes](https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/8b8f9ec9-65bf-419b-b205-856d36018960)


## Model Selection

Selecting an appropriate machine learning library is crucial. Popular libraries such as Scikit-learn (sklearn), TensorFlow, Keras, 
and XGBoost were considered. Scikit-learn was chosen for its robustness, extensive online resources, ease of learning, and the 
availability of various algorithms for comparison.

## Results
- **LinearRegression**
score: 0.0106,
execution time: 4.9s  <br>
- **LogisticRegression**
score: 0.998,
execution time: 11.4s  <br>
- **DecisionTreeRegressor**
score: 0.4679,
execution time: 29.9s  <br>
- **RandomForestClassifier**
score: 0.9995,
execution time: 14m 41.2s  <br>

<p align="left">
  <img width="500" height="500" src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/dd18977b-6237-4323-a326-29150e7bed88"> </p>


We also analyze feature importance of the RandomForrestClassifier.

![image](https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/eb9a27db-a9ad-46ef-8092-42fc2883362e)

## Conclusion

We developed a classification model using Kaggle.com's dataset to predict fraudulent transactions. Among the 
algorithms tested, Logistic Regression and Random Forest proved to be the most accurate, achieving a remarkable 
99% prediction accuracy on the test set. Notably, Logistic Regression demonstrated greater efficiency despite dealing 
with an unbalanced dataset, resulting in effective fraud prediction.

---
