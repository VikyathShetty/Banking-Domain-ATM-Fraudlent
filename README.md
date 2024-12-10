
#  Banking Domain Fraudulent Detection System 

This project is a banking domain application specifically developed to detect and flag fraudulent transactions in financial data. The system processes transactional data and classifies each transaction as either clean or fraudulent. For clarity and consistency in the output, the program has been enhanced to represent clean (legitimate) transactions with the value 0 and fraudulent transactions with the value 1. This approach ensures easy integration with downstream systems and facilitates quick analysis of transaction statuses.


## Documentation
### Train and Test Datasets:

Separate datasets used for model training and evaluation. These datasets contain historical transaction data that are essential for training the machine learning models to detect fraudulent transactions.

### Geo_Scores:

This dataset stores location data, indicating where each transaction took place. It helps in assessing the geographical risk associated with transactions, providing additional context to detect suspicious activities based on transaction location.

### Lambda_Wts:

This dataset includes information regarding individuals or groups, identified by a unique ID. It is used to track and assess transaction patterns for similar persons or groups, aiding in identifying potential fraudulent behavior based on group-level analysis.

### Instance Scores:

This dataset contains numerical values representing the risk or quality associated with a particular transaction, customer, or data instance. The score helps in evaluating the likelihood of fraud and the overall risk profile of each entity.

### QSET_TATS:

This dataset provides detailed information such as transaction counts, transaction types, and other relevant metrics for each account. It helps in understanding transaction behavior and identifying anomalies that may indicate fraudulent activities.

[Dataset](https://github.com/VikyathShetty/Banking-Domain-ATM-Fraudlent)



