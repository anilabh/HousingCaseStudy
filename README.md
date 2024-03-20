## Housing Price Prediction


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
We are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

- What is the background of your project?
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. 

- What is the business probem that your project is trying to solve?
The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

Which variables are significant in predicting the price of a house, and how well those variables describe the price of a house. Also, determine the optimal value of lambda for ridge and lasso regression.

- What is the dataset that is being used?
The data given in a csv contains information about sale of houses in Australia and parameters about the houses describing area, build quality , surroundings etc.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->
Lasso with alpha 0.0001 shows the best R2 on Test Set. Optimal alpha for Ridge is 0.7

Top predictor variables selected by Lasso regression:

1stFlrSF 0.227597
OverallQual 0.218375
OverallCond 0.101245
2ndFlrSF 0.094950
GarageArea 0.089978
LotArea 0.063677
TotRmsAbvGrd 0.058231
BsmtFullBath 0.049152
FullBath 0.043161
FireplaceQu 0.036543

1st floor area is the most important variable in predicting the Sale Price. This is followed by overall quality and over all condition of the house. Overall area plays a key factor as is reflected by 2nd Floor, Garage and Lot areas being in the top 6 variables.

We see an almost linear graph between predicted and observed target variable on test set.

This means our model is able to predict the test data quite well

Nominal variable analysis shows that high Sale Price is associated with:

Cement Board or Stone for Exterior covering
Builtin Garage
SaleType of : Newly build and sold and Contract 15% Down payment regular terms
Neighborhood type of Northridge and Northridge Heights
Foundation with Poured Concrete
Sale Condition Partial : Home was not completed when last assessed (associated with New Homes)

...and low Sale Price is associated with:

Commercial zones
Asbestos Shingles exterior covering
No garage
Neighborhood type of Meadow Village
Brick Common type of Exterior covering
Foundation with Slabs
Sale Condition with Adjoining Land Purchase

## Technologies Used
- Python 3.11.1
- Pandas 2.1.4
- Numpy 1.26.3 
- Seaborn 0.13.1
- Sklearn 1.4.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@anilabh]


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->