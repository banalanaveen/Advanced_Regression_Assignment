# Surprise Housing - Problem Statement
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file attached.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

* Which variables are significant in predicting the price of a house, and

* How well those variables describe the price of a house.


## Table of Contents
* Reading and Understanding Data
* EDA and Visualising the Data
* Model Building with feature selection using RFE
* Ridge Regression
* Lasso Regression
* Conclusion

## Business Goal 

> You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Conclusions
- we got very good score for both Ridge and Lasso Regression

    Metric             Linear Regression  Ridge Regression  Lasso Regression
    
    R2 Score(Train)        0.949801            0.915192         0.900741
    
    R2 Score (Test)        0.862228            0.889950         0.886565 


Top5 most significant features in Ridge are:

* ('SaleType_Oth', 0.063),
* ('SaleType_WD', 0.067),
* ('SaleCondition_Normal', 0.085),
* ('SaleCondition_Others', 0.09),
* ('SaleCondition_Partial', 0.099)


Top5 most significant features in Lasso are:

* ('SaleType_Oth', 0.065),
* ('SaleType_WD', 0.072),
* ('SaleCondition_Normal', 0.097),
* ('SaleCondition_Others', 0.101),
* ('SaleCondition_Partial', 0.106)



##Optimal Value of lamda for Ridge is 10

##Optimal Value of lamda for Lasso is 0.001


Ridge Regression did better than Lasso Regression when R2 is compared.

RSS Values of Ridge Regression and Lasso Regression are small for test than train set, where for Linear regression is more for test set.

Ridge did better even with RSS values when compared to Lasso.



## Contact
Created by [github.com/banalanaveen] - feel free to contact me!


