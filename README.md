# FraudulentTransactions
# Fraud Detection Project

This project focuses on detecting fraudulent transactions using a variety of transaction-related features, including transaction type, amount, customer information, and AML (Anti-Money Laundering) risk flags. The core of the project is built around a Python class, `ModelTrainer`, which encapsulates data preprocessing, model training, hyperparameter tuning, and feature importance analysis.

Dataset Description
The model expects the following features in the dataset:

transaction_amount: The amount of money involved in the transaction.
transaction_type: The type of transaction (e.g., online, in-store, mobile).
customer_address: The customer's address category (e.g., Urban, Suburban, Rural).
customer_email_domain: The domain of the customer's email address.
customer_bank_account: Type of customer's bank account (e.g., Bank A, Bank B).
country: The country where the transaction took place.
aml_risk_flag: Flag indicating whether the transaction was flagged by an AML system.
is_fraud: Target variable indicating whether the transaction is fraudulent.

Model
This project uses a RandomForestClassifier model to predict fraudulent transactions. It includes preprocessing steps for handling numerical and categorical data and employs GridSearchCV for hyperparameter tuning. The ModelTrainer class facilitates the entire workflow from data loading to model evaluation.
