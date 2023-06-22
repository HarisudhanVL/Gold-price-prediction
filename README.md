# Gold-price-prediction using Regression Techniques

## Problem Description:
* In present times, precious metals like gold are held with central banks of all countries to guarantee repayment of foreign debts.
* The problem is based on gold rate prediction.
* The gold price is dependent on various other factors like price of other precious metals (silver, platinum, etc…), price of crude oil, stock exchange performance, currency exchange rates etc…

## Goal:
* The main objective is to predict the daily rise and fall in gold rates which can help the investors to decide when to buy or sell the commodity.
* The challenge is to predict the future adjusted closing price of gold ETF (exchange trade fund).

## DATASET DESCRIPTION
* The data for this study is collected from 18th Nov 2011 to 1st Jan 2019 from various sources.
* The dataset is from YAHOO FINANCE.
* The dataset contains 1718 rows and  80 features in total.
* The index consists of individual days and the target feature is “Adj Close”.
* Data for attributes, Oil price, Standard and poor's (S&P) 500 index, Dow Jones index US bond, Euro USD exchange rates, Prices of US dollar index, Eldorado Gold Corporation, Gold miners, Price of precious metals.

Sample data from dataset,

![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/ac34e728-872d-4ad0-934b-9490806cc866)
![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/c9a5e23c-2b37-49b1-9637-8a8e42559745)

ML procedure done for this project
1. Exploratory Data Analysis

![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/925e494a-b86b-4a83-bff0-c2e6c385da51)
From the end of 2011 to early of 2016 the price was in downward trend. In 2016 to 2018 the price was between 110 to 130.
2. Data Preprocessing
* Dropped the higly co-related varibales
* Dropped the very less correlated features.
* Detected skewness and normalized. For example
Left Skewed,

![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/a3a4e2a9-83e7-4f8c-b9cc-dbcb271e3c4c)

After applied normalization,

![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/cbe4a9cc-5b7e-468e-a5b2-f7c8cd4fea27)
* Separate the dependent and independent variables.
* Scale the data.
* Calculate variance ratio.
* Plot the cummulative variance plot with explained variance of threshold 95%.

![image](https://github.com/HarisudhanVL/Gold-price-prediction/assets/68286374/0ea5de7e-ab63-44b9-956f-3522a77fc5bc)

Observe the above plot clearly, the 95% threshold line exactly cuts the variance curve at n_components = 7, so the the features can be reduced to 7 components.

* Apply PCA to the features

3. Build the ML model
4. Evaluate the performance of the model.

### For you further clarity please look into notebook file.
