# Advanced Regression Model for Surprise Housing
> This assignment is a programming model wherein we are building a Ridge and Lasso regression model for the price of houses with the available independent variables.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
- A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

- The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

- The company wants to know:

> 1. Which variables are significant in predicting the price of a house, and
> 2. How well those variables describe the price of a house.
 
Also, determine the optimal value of lambda for ridge and lasso regression.


## Conclusions
-  From the Results, It is clear that Ridge and Lasso performing better than the Linear model when the Overfitting present.
-  Also Lasso model gives better regularization than ridge for the optimal value of lambda for the given dataset. This is due to some of the variable might not be significant in predicting the target variable and Lasso handling that by zeroing out the coefficient value of those variables which result in the feature selection.

-  #### From the beta value of Ridge model,
> 1. 1stFlrSF (First Floor square feet)
> 2. GrLivArea (Above grade (ground) living area square feet)
> 3. BsmtFinSF1 (Type 1 Basement finished square feet)
> 4. TotalBsmtSF (Total square feet of basement area)
> 5. OverallQual_9 (the overall material and finish of the house which is Excellent)

Theses are the top 5 significant Independent variables in explaining the target variable.

- #### From the Beta values of Lasso Regression, 
> 1. GrLivArea(Above grade (ground) living area square feet)
> 2. OverallQual_9 (the overall material and finish of the house which is Excellent)
> 3. OverallQual_10 (the overall material and finish of the house which is Very Excellent)
> 4. TotalBsmtSF (Total basement area in Square feet)
> 5. Years_since_Built ( Which is a derived metrics, No of years since the property built)

This are the 5 most important significant variables. In this, Years_since_Built variable is negatively affecting the target varibale with negative coefficient value.


## Technologies Used
- Pandas
- Numpy
- Seaborn
- Matplotlib
- statsmodel
- sklearn

## Contact
Created by [@baranitharan16] 
