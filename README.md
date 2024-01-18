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



 - [Data Cleaning](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#data-cleaning)
     - [DESCR Column](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#descr-column)
     - [HIRE_DT Column](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#hire_dt-column)
     - [Filtering Data](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#filtering-data-for-one-department-descr-column)
 - [Simple Linear Regression](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#simple-linear-regression-1)
     - [Least Squares Line](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#least-squares-line)
     - [Calculating Errors](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#calculating-errors)
     - [Standard Error of Residual and Outliers](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#standard-error-of-residual-and-outliers)
 - [Further Analysis](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example#further-analysis)
 
 The original files were exported from the [Baltimore City Open Data portal](https://data.baltimorecity.gov/City-Government/Baltimore-City-Employee-Salaries-FY2018/biyh-j8tc), and are available in this repository as an [Excel](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example/blob/master/Baltimore_City_Employee_Salaries_FY2018.xlsx) document and as a [CSV document](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example/blob/master/Baltimore_City_Employee_Salaries_FY2018.csv). The final excel document with the example covered in this tutorial is also available in this repository as an [Excel document](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example/blob/master/Baltimore_City_Employee_Salaries_FY2018_bus_analytics_in_class_simple_reg.xlsx).
