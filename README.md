# fuzzylogic_repo

This is the repository for rakamin batch 18 final project, focusing on loan prediction based on customer behavior.

### Intro
A fintech company has a dataset which consists of customers info and behavior and whether these customers were able to repay the loan back or not. From this data, they want to predict what type of customers that can be a possible dafaulters. The prediction will be used to avoid giving loans to these type of customers.

### About Data
Data consists of 13 columns, with 1 target feature (risk_flag)

### Preprocessing
 * There are no missing data or duplicated data.
 * There are no outliers in the dataset.
 * Feature encoding is aplied to 8 columns, with 4 using label encoding, 1 using one hot encoding, and 3 using frequency encoding.
 * Imbalanced data on the risk_flag feature is handled with the SMOTE technique.

### Modelling and Evaluating
Model is evaluated on the basis of recall and AUC score, while considering the execution time. Therefore, the best suitable model is Decision Tree with **recall = 0.831** and  **AUC = 0.873** (after hypertuning).
