# Phase-3-Project
Author : Elsie Lovell Kiprop

![image](https://user-images.githubusercontent.com/104361809/182010063-4dd85098-6e86-4e44-9d8f-c6fae586dfa4.png)

## Overview
SyriaTel is a mobile network provider based in Syria with a customer base of over 8 million.
This project analyses data to check for factors that lead to churning of customers. The project seeks to investigate customer retention in order to minimise their losses.

## Business Understanding
Being a telecommunications company, retaining customers is very important for SyriaTel to make profits.SyriaTel is interested in reducing the losses that arise due to customers quitting using their services after a given time.

Therefore, this project will aim to investigate customer churn which simply means the percentage at which the customers stop using a company over a specific period of time. This will help SyriaTel,who is our stakeholder to cut down the losses made when some customers quit using their services. It will also be important in finding the factors that greatly influence customer churn.

## Data Understanding 
The data used was sourced from Kaggle. Its called ```bigml_59c28831336c6604c800002a.csv```. 

The dataset contains the following columns:
* state
* account length
* area code
* phone number
* international plan
* voice plan
* number vmail messages
* total day minutes
* total day calls
* total day charge
* total eve minutes
* total eve calls
* total eve charge
* total night minutes
* total night calls
* total night charge
* total intl minutes
* total intl call
* total intl charge
* customer service calls
* churn

The target variable in this case is ```churn``` where false(0) represents a customer not quiting SyriaTel's services while true(1) represents a customer quiting the services.

## Method
Jupyter notebook was used in this project. Various steps were carried out in the analysis of the data. They include:
* Data Cleaning
* Exploratory Data Analysis.
* Data Preprocessing
* Modelling- Involved creating a  number of models and hyperparameter tuning
* Drawing conlusions and providing recommendations

## Final Model
There were a number of various models created which included : Logistic regression, Random Forest, Decision Trees and K Nearest Neighbors. Each of these models were evaluated  before and afer hyperparameter tuning. The best performing model was picked as the final model. The best model was the base Random Forest Regression model. The following were its metrics:
* **Accuracy = 0.9520383693045563**
* **Recall = 0.712**
* **F1 score = 0.81651376146789**
* **Precision = 0.956989247311828**
* **AUC = 0.853179125528914**

Having chosen our model, I also investigated feature importance in order to provide optimal recommendations. The following is a visualization of the feature importance in ascending order:

![image](https://user-images.githubusercontent.com/104361809/182009495-8f28239e-a937-4e94-b338-5d00be06ee79.png)

## Summary
The top 5 factors that influenced churning are:
* Total day charge
* Customer service calls
* Total eve charge
* International plan
* Total international charge

## Reccomendations and Conclusion
The recommendations given included:
* Analysing customer service call to know what issues customers raise and make appropriate adjustments. They should also make follow ups to see if those who made calls were helped.
* Reducing day, eve and international charges in order to retain customers. Additionally they could give bonuses to thoses who use theire services more: for example free minutes or calls.
* Come up with a favourable international plan or alternatively get rid of the product since majority of the customers do not subscribe to it.

Having these recommendations, after implementing them, Syriatel should later evaluate them and check whether the changes they made are effective and check whether they are cost effective.
