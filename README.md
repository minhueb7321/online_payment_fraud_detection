# Online Payment Fraud Detection

## Description
Online payment is the most popular transaction method in the world today. However, with an increase in online payments also comes a rise in payment fraud. The objective of this study is to identify fraudulent and non-fraudulent payments. The dataset is collected from Kaggle, which contains historical information about fraudulent transactions which can be used to detect fraud in online payments.

## Dataset Overview
The dataset consists of 10 variables:

- `step`: represents a unit of time where 1 step equals 1 hour
- `type`: type of online transaction
- `amount`: the amount of the transaction
- `nameOrig`: customer starting the transaction
- `oldbalanceOrg`: balance before the transaction
- `newbalanceOrig`: balance after the transaction
- `nameDest`: recipient of the transaction
- `oldbalanceDest`: initial balance of recipient before the transaction
- `newbalanceDest`: the new balance of recipient after the transaction
- `isFraud`: fraud transaction

This project detects online payment fraud using machine learning techniques on Google Colab. Key features include:
- Applying SMOTE for class imbalance, along with preprocessing steps like scaling, label encoding, and outlier treatment.
- Developing fraud detection models using Logistic Regression, Random Forest, SVC, and XGBoost, achieving 98% recall and 98% accuracy with the best model (XGBoost).
- The project is contained in a single file, which includes code and dataset.

The dataset is sourced from Kaggle.

## Project Structure
```
online_payment_fraud_detection/
├── online_payment_fraud_detection.zip  
├── notebooks/                         
│   └── fraud_detection.ipynb
├── data/                            
│   └── dataset.csv
├── requirements.txt                 
```

## How to Use
### 1. Set Up Environment on Colab
- Download the `online_payment_fraud_detection.zip` file from this repository.
- Upload the ZIP file to Google Colab.
- Unzip the file in Colab by running:
  ```
  !unzip online_payment_fraud_detection.zip -d .
  ```
- Install required libraries by running:
  ```
  !pip install -r requirements.txt
  ```

### 2. Run the Project
- Open the `fraud_detection.ipynb` file in Colab (after unzipping).
- Execute the cells to preprocess data, train models, and evaluate performance.
- If the dataset is embedded, no additional upload is needed.

## Requirements
- Google Colab environment.
- Python libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `imbalanced-learn`.

## Dataset
- Source: Kaggle [https://www.kaggle.com/code/seuwenfei/online-payment-fraud-detection/input].
- Included within the ZIP file or notebook.


