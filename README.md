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

- Likewise we have created pivot table for [Tenure], [Gender] and [Georgraphy] with [ChurnRate] and [CreditScore]

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot2.png)

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot3.png)

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/4e3b8f96549da6884b37e2921602a80bc79d9732/Pivot4.png)

- Conclusion drawn is,
  - the highest no of products holder are tend to exit.
  - Initial years(0, 1) customers ChurnRate is the highest.
  - Female customers ChurnRate compared to Male is highest.
  - Geographically, Germany's ChurnRate is highest against Spain and France.

With this information we can come up with the best subscription plans for these users.  


# Regression Analysis
- The target variable(dependent variable) is [Exited] to analysis the best independent variable explains about this variable we performed statistic regression using Data analysis in built tool in Excel.

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/8eacec2c83b182301b9bfa681adfbde0396cc589/RegressionS1.png)

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/8eacec2c83b182301b9bfa681adfbde0396cc589/RegressionS2.png)

![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/8eacec2c83b182301b9bfa681adfbde0396cc589/RegM1.png)
![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/fd64072f167827c116dd25cb6589694c1304abc2/RegOutput.png)
![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/8eacec2c83b182301b9bfa681adfbde0396cc589/RegFinalM.png)


![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/fd64072f167827c116dd25cb6589694c1304abc2/BestfitlineGraph.png)



![Alt Text](https://github.com/mrunalibharshankar/RegressionAnalysis/blob/fd64072f167827c116dd25cb6589694c1304abc2/Calculation.png)

# Conclusion:  
1. Statistical Significance:

Researchers assess the statistical significance of the coefficients. A coefficient is considered statistically significant if its p-value is below a predetermined significance level (e.g., 0.05). This helps determine if there is a significant relationship between the independent and dependent variables.
Coefficient Interpretation:

The sign and magnitude of the coefficients are interpreted. A positive sign indicates a positive relationship, while a negative sign indicates a negative relationship. The magnitude indicates the strength of the relationship.
Predictive Power:

The overall predictive power of the model is assessed using metrics like R-squared. A higher R-squared value suggests that the independent variables explain a larger proportion of the variance in the dependent variable.
Variable Importance:

Researchers may identify which independent variables are most important in explaining the variability in the dependent variable. This is based on the magnitude of the coefficients and their statistical significance.
Model Fit:

The overall fit of the model to the data is evaluated. Residual analysis helps assess how well the model's predictions align with the observed data.
Assumptions Check:

Researchers check whether the assumptions of regression analysis are met, including linearity, independence of errors, homoscedasticity, and normality of residuals. Violations of these assumptions can impact the validity of the conclusions.
Outlier Detection:

Outliers are identified and their impact on the results is assessed. Outliers can influence the estimated coefficients and may need special attention.
Generalization:

Conclusions drawn from the analysis are considered in the broader context. Researchers may discuss the generalizability of the findings to a larger population or different settings.
It's important to note that regression analysis provides insights into associations and relationships, but it does not imply causation. Conclusions should be drawn cautiously, considering the study design, limitations, and the appropriateness of the model for the given data.
    


  

  
















