
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


## Data Preprocessing and Merging
### Concatenating Train and Test Data:

The train and test datasets are combined into a single dataset to facilitate consistent preprocessing and analysis. This merged dataset serves as the primary data source for model training and evaluation.

### Handling Missing Values:

To manage missing values, we replace them with the median value present in the respective columns of the dataset. This approach helps maintain the integrity of the data and ensures the model is trained on a complete dataset.

### Merging Geo_Scores:

Geo_Scores are combined with the main dataset based on a unique identifier (ID). This merging ensures that the number of columns is consistent across all datasets, allowing for a unified dataset structure.

### Merging Lambda_Wts:

The Lambda_Wts dataset, which contains data regarding individuals or groups identified by a unique ID, is merged with the main dataset similarly to Geo_Scores. This step allows for group-level analysis and tracking of transaction patterns.

### Merging Instance Scores:

Instance Scores, which represent the risk or quality associated with a particular transaction, customer, or data instance, are merged based on the ID of the group or individual. This helps in 
assessing the overall risk profile of each entity in the dataset.

### Final Dataset Structure:

After merging all datasets on the basis of the ID, we have a consolidated dataset with all relevant columns, ready for analysis and model training


## Heatmap

![heatmap is a useful tool for visualizing the correlation between columns in a dataset.](https://github.com/VikyathShetty/Banking-Domain-ATM-Fraudlent/blob/main/images/Screenshot%202024-12-10%20115522.png)

## Machine Learning Models and Evaluation
In this project, the training data was split into feature variables (X) and target variable (y) for training and testing purposes. We then applied six different machine learning models to determine which one provided the best performance in terms of accuracy. 

The models used are:

**Logistic Regression**

**Support Vector Machine (SVM)**

**K-Nearest Neighbors (KNN)**

**Decision Tree**

**Random Forest**

**Voting Classifier**

After evaluating all the models, the Random Forest classifier yielded the highest accuracy, outperforming the other models.
## Vislual Representation 

![BarPlot to check accuracy of the model](https://github.com/VikyathShetty/Banking-Domain-ATM-Fraudlent/blob/main/images/Screenshot%202024-12-10%20120556.png)


