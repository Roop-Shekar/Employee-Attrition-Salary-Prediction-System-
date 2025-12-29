
# Employee Attrition & Salary Prediction System README
The project is aimed at forecasting employee turnover and estimating the financial consequences of employee turnover through the use of machine learning. This is aimed at assisting the organizations to identify high-risk employees proactively and quantify the possible loss of money due to attrition.

##DATASET LINK: https://www.kaggle.com/datasets/patelprashant/employee-attrition


##  Project Overview
The phenomenon of employee attrition is a burning issue that organizations have to contend with because it causes higher expenses in hiring, wastage of productivity, and knowledge base.  
The models used in this project using machine learning include:
Anticipate whether an employee will quit the organization or not.
Project future remuneration of employees that will remain.
Estimate the loss in finance that is likely to occur as a result of possible defection.
The project is based on the IBMS HR Analytics Employee Attrition Dataset.

## Dataset Information
 Data: IBM HR Analytics Employee Attrition Dataset.  
 Total Records: 1470  
 Features: 35  
 Target Variable: Yes / No
The data includes the demographics of the employees, job description, performance and salary.

##  Methodology

###  Data Preprocessing
 Categorical features supplied by the use of a LabelEncoder.
 Columns that are irrelevant were dropped ( `EmployeeNumber, StandardHours, Over18, EmployeeCount)
 StandardScaler used to perform feature scaling.
Predicts if a user will attrit or not, regardless of whether they become a customer.<|human|>Predicates the propensity of a user to attrit or not, whether or not they will become a customer.
Model Used: Logistic Regression
Train-test split: 80% / 20% 
Evaluation Metrics:
F1 Score
ROC-AUC Score

The model forecasts the possibility of an employee dropping out of the organization.
Salary forecasting involves a regression-based method that employs the assumption that variations in independent variables significantly influence the dependent variable.<|human|>Salary Forecasting (Regression) . This is a regression-based approach that assumes the existence of significant variation in both the independent and dependent variables.
To the employees who are expected to remain: Raise in salary depending on performance rating:
Rating = 4 then 10% increment
Otherwise  5% increment

Random Forest Regressor was trained to forecast future values of salaries.

Evaluation Metrics:
R² Score
RMSE (Root Mean Squared Error)

###  Financial Loss Estimation
The estimation of expected financial loss is done by using:
Future Salary × Probability of Attrition = Expected Loss.
This will allow in quantifying the business potential of employee attrition.
##  Results Summary
 Logistic Regression AUC-ROC: ~0.77
Logistic Regression F1 Score: ~0.47
Regression R 2 of random forest: ** 0.99: Total Financial Loss: 12,42,813(approx.)

##  Tools & Technologies Used
Python
Pandas
NumPy
Scikit-learn
Jupyter Notebook

