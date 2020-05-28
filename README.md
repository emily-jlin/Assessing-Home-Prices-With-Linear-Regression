# Assessing the Home Prices of Ames, Iowa Using Linear Regression Model

## Problem Statement
To determine the appropriate predictors that affect housing prices and use linear regression model to predict the housing prices as accurately as possible.

## Executive Summary
This project aims to understand the factors that affect the sales price of houses in Ames, Iowa using data collected by Ames Assessor’s Office from 2006 to 2010. This dataset has 2920 rows and 82 variables with "23 nominal, 23 ordinal, 14 discrete, and 20 continuous variables (and 2 additional observation identifiers)"(1). The objective of this project is to determine the appropriate predictors and use linear regression to assess the housing prices using these predictors.

The Ames Accessor's Office's responsibility is to assess constituents' properties as accurately as possible as new housing developments emerge, real estate propertities transfer, and the value of houses appreciates or depreciates. The accessor's office holds key decision making power in deciding the value of real estates that impact property taxes and real estate transfer taxes that are crucial to Ames' tax revenues and affect residents' financial decisions.

The modeling process for linear regression starts with data cleaning. Provided below is the sample data dictionary that helps readers to walk through the project and use as a guide in the data cleaning process. During the data cleaning process, readers can find the codes for each ordinal category labeled using conventional such as renaming "Excellent" to 4 and "Poor" to 0. After categorizing data, readers can find graphs that visualize the relationship between each variable and the sales price of houses. Lastly, a linear regression model is fitted to the data.

The above process is not a one-way street, rather an iterative process. The following table of contents separated each section to help readers to refer back to another step conveniently.

## Table of Contents
<<<<<<< HEAD
-Importing Data
-Cleaning Data
-Categorizing Ordinal Data
-Exploratory Data Analysis
-Linear Regression Modeling
-Lasso
-Hypothesis Testing
-Conclusion and Recommendation


## Exploratory Data Analysis
![Part one EDA]('img/eda1.png')


![Part two EDA]('img/eda2.png')


![Kitchen Quality]('img/kitchenquality.png')


![Kitchen Quality]('img/paveddrive.png')
=======
- Importing Data
- Cleaning Data
- Categorizing Ordinal Data
- Exploratory Data Analysis
- Linear Regression Modeling
- Lasso
- Hypothesis Testing
- Conclusion and Recommendation

## Exploratory Data Analysis

Below are some graphs that are used in the EDA process to help me identify trends and relevant predictors.
![](http://url/to/img.png)
>>>>>>> 3a13bf25609f7a9bd59027ffaf25619ba1cd192b

## Conclusion and Recommendation
|Predictors|% Change in Sale Price if Predictor is Increased by 1 Unit|
|-|-|
|Central Air|16.66%|
|Neighborhood Codes|15.15%|
|Paved|11.4%|
|Overall Quality|8.75%|
|Sale Type (New or Con)|7.39%|
|Kitchen Quality|6.25%|
|Electrical|2.29%|
|1st Floor Square Foot|0.028%|
|2nd Floor SF|0.023%|
|Garage Area|0.014%|
|Type 1 finished square feet |0.012% |
|Total Basement Square Foot|0.008%|
|Mason Veneer Area|-0.0026%|
|General Living Area|0.0025%|

The above chart highlights the 14 predictors that are used in this model to assess the housing prices in Ames. While it is easy to conclude that the predictor with the highest percentage change in sale price is the strongest influencer, it is important to quantify each predictor before making that conclusion. For example, Central Air is a categorical data that contains two data points: 0 or 1. 0 for houses without central air and 1 for houses with central air. With values that are 0 or 1, it is more likely that the percentage change is inflated that it actually is in real life. Another way to quantify the predictors is to consider the real life application. For example, general living area has the lowest percentage, but the predictors also have the highest range. Let's take a house that is selling for 500,000 dollars, if the general living area's square footage is increased by 1 unit, the sale price is predicted to increase by 500,000 * 1.0025 = 501,250 dollars, with all else hold equal. A typical bedroom size is about 132 square foot so general living area actually has a greater influence than central air.

Two of the predictors here are especially susceptible to data entry errors or bias during rating: Kitchen Quality and Overall Quality. It is paramount for Ames Assessor's Office to ensure that all their agents understand the guidelines on how to rate each house and standardize the rating rubric to minimize bias. In addition, the office should consider cross validating each agent's scores by sending two or three agents to evaluate the house to prevent bias. The Ames Assessor's Office's evaluation is crucial to the wealth of the city and residents. Taking these precautionary steps to validate the data will ensure that the model perform optimally to assess housing prices as accurate as possible.
