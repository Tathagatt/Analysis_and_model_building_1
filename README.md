## PROBLEM STATEMENT
The main goal of the problem is to develop a machine learning algorithm that predicts the scout-made evaluation of players in the context of given matches.
## APPROACH
## Data Analysis – 
•	 I performed this step to understand more about the data like the shape of the data, the datatypes of different features. There were more than 700 features so needed feature selection and feature decomposition to decrease the complexity of the dataset.
•	 After this used “isnull ()” operation to know which features have null values and imputed these null values by replacing them with median values.
•	 Then dropped columns with all the values as null and also dropped those columns with more than 90% of 0 values. 
•	 Dropped columns with standard deviation smaller than 0.05.
•	 Encoded two nominal categorical features.
## Feature Engineering – 
•	 Used the p-value for feature selection and LASSO regularization to decrease the complexity of the model. After all the feature selection techniques, around 300 features were selected from 800 features. 
•	 Handled the outliers using IQR technique in which replaced all the lower outliers with lower bound value and all he higher outliers with higher bound value.
•	 Changed the label a bit to increase the accuracy and meet with the results.
•	 Used clustering algorithm too but it was not giving any good results.
## Model Finder – 
•	 Used Logistic Regression at first but the score was not good.
•	 Then used Random Forest with some hyper parameters tuning and got the prediction where 1 score was good but not good enough. 
•	 At last used XGBOOST Regressor and got the best r2 score in all the submission.

 
