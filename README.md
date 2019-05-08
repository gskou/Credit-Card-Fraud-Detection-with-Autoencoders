# Credit-Card-Fraud-Detection-with-Autoencoders
Classification model that predicts fraudulent transactions 

You can find more info regarding the data and the project on Kaggle.
https://www.kaggle.com/mlg-ulb/creditcardfraud


Content

On Kaggle we read:
"The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise."

Why Autoencoders?

There are two important benefits in using autoencoders over other type of classification algorithms:

1)Imbalance of the data.
The dataset is quite imbalanced since the majority of the observations are normal data.
However, when training an autoencoder we need only normal transcaction. That is because when we add new observations to the model it will be able to classify not well predicted observations as fraudulent ones. 

2)Anomalies detection is not trained for a specific type of anomaly
That means that anything that is different from normal can be detected and classified accordingly. 
