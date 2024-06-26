# Credit-Card-Fraud-Detection
## Problem statement
The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of machine learning models.

In this project, we will analyse customer-level data which has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group.

The dataset is taken from the [Kaggle website](https://www.kaggle.com/) and it has a total of 2,84,807 transactions, out of which 492 are fraudulent. Since the dataset is highly imbalanced, so it needs to be handled before model building.
## Data Dictionary
The dataset can be download using this [link](https://www.kaggle.com/datasets/joebeachcapital/credit-card-fraud)

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from **‘time’** and **‘amount’**, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature **'time'** contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature **'amount'** is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.
## Project Pipeline
The project pipeline can be briefly summarized in the following four steps:

- **Data Understanding**: Here, we need to load the data and understand the features present in it. This would help us choose the features that we will need for your final model.
- **Exploratory data analytics (EDA)**: Normally, in this step, we need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, we do not need to perform Z-scaling. However, you can check if there is any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.
- **Train/Test Split**: Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation, we can use the k-fold cross-validation method.
- **Model-Building/Hyperparameter Tuning**: This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given dataset.
- **Model Evaluation**: We need to evaluate the models using appropriate evaluation metrics.
