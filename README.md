# Regression Analysis in Excel

# Overview
This dataset is for ABC Multistate bank with following columns:

- _RowNumber_, unique no.
- _CustomerId_, unique id represents the individual customer.
- _Surname_, last name of the customer
- _CreditScore_, number that measures customers risk.
- _Geography_, country the customer is based, and its categorical variable.
- _Gender_, Female or Male, its categorical variable.
- _Age_, age of the person.
- _Tenure_, for how many years the customer is with the bank.
- _Balance_, available amount for withdrawals.
- _NumOfProducts_, no of products the customer has and, its a categorical variable.
- _HasCrCard_, if customer owes credit card. 1 for yes and 0 for no.
- _IsActiveMember_, 1 for he/she is active and 0 for not active.
- _EstimatedSalary_, Salary.
- _Exited, 1 if the client has left the bank and 0 if he/she has not. Its the target 
       variable.

The original files were exported from the [Kaggle](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset), and are available in this repository as an [Excel](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/main/Churn_Modelling1.xls) document.

Regression analysis is a statistical technique used to examine the relationship between one dependent variable and one or more independent variables. The goal is to understand how the independent variables impact the dependent variable.

For Regression Analysis to approximate how two variables in a dataset are related. In the following dataset for regression, we’ll have:
- An independent variable, which is explanatory variable. This variable can be directly controlled.
- A dependent variable, which is target variable. This variable cannot be directly controlled, and can depend on independent variable.

The general form of a regression equation is:
 **Y= β0 + β1*X1 +β2X2+…+βnXn + ϵ**

- Y is the dependent variable.
- X1,X2,..Xn are independent variables.
- β0 is the y-intercept.
- β1, β2,..βn are coefficients representing the relationship between the independent and dependent variables.
- ϵ is the error term.

The general line graph, that independent variable runs along the x-axis, and dependent variable runs along the y-axis
![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/24c43203a0b58bc66dd831b17bf089f5d2a44fe4/line_example.png)


The regression analysis aims to estimate the coefficients (β) that minimize the difference between the observed and predicted values of the dependent variable.

Key concepts associated with regression analysis include:

- _R-squared (R²)_: Indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.
- _Coefficients_: Represent the strength and direction of the relationship between the independent and dependent variables.
- _Residuals_: The differences between the observed and predicted values.


# Transforming Variable
- Added [total_counter] column by using countif() function of excel to count the duplicate records against the CustomerId column which represents the unique records.
  
![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/94fa03a3d1f4c10b5b602dc80acde987232b5910/total_counter.png)

# Pivot Analysis
- Created new field list ChurnRate by dividing [Exited]/[total_counter] to find out [Sum_of_Churnrate]
- First analysis was to draw conclusion of [NoOfProducts] against [ChurnRate] and [CreditScore]
  
![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/6d9b6a9250941794aa4b910593eb6d9804a586f7/Pivot1.png)
- Conclusion drawn is, the highest no of products holder are tend to exit.




![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot2.png)


![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot3.png)

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot4.png)




  

  
















