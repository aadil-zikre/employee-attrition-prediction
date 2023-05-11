# employee-attrition-prediction
Attempting to predict whether an employee will leave the company

## Dataset 
Taken from Kaggle : https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

## Process
Following things were done for building a predictive model for predicting if an employee is going to leave the organization:
1. EDA - Various Visualizations to find patterns visually
2. Feature Reduction - By making a correlation matrix, features that were too highly correlated or had no variance at all were removed
3. Train Test Split - 25% of the dataset was held out for testing
4. 3 Models were trained - Decision Tree, Random Forest, XGBoost
5. 5 fold Cross Validation was used to train the models
6. Grid Search CV was used to tune the hyperparameters. A separate HyperParameter space was defined for each Model 
7. Model performances were evaluated using weighted f1 score. XGBoost performed the best with 86% Accuracy

## Conclusion
Xgboost Feature Importance curve revealed compensation, hike and job satisfaction to be the major contributors to attrition of employees. Therefore, HRs should focus more on these factors when trying to retain employees. 
