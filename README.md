# Regression Analysis in Excel

# Overview
This dataset is for ABC Multistate bank with following columns:

_customer_id_, unused variable.
_credit_score_, used as input.
_country_, used as input.
_gender_, used as input.
_age_, used as input.
_tenure_, used as input.
_balance_, used as input.
_products_number_, used as input.
_credit_card_, used as input.
_active_member_, used as input.
_estimated_salary_, used as input.
_exited_, used as the target. 1 if the client has left the bank and 0 if he/she has not.


 - [Overview](https://github.com/jhu-business-analytics/simple-linear-regression-excel-example/blob/master/README.md#overview)
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
