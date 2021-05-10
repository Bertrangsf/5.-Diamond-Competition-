![portada](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTN2YGZOtVL_z4hy-CPYqVsFP10HX0oSzp2Kw&usqp=CAU)

# PROJECT: Diamond Competition 

## Overview

Like all gemstones, diamonds have several characteristics that determine their value. In this project, all of them had to be considered in order to determine the optimal model for determining the price of a diamond. We were given two .csv's, one with the characteristics and the price (with which we were to create the model) and one with the characteristics without the price (to apply the models and try to find out the price based on those characteristics). 


## Table of Contents
1. [General Info](#general-info)
2. [Data treatment](#Data-treatment)
3. [Libraries](#Libraries)
4. [Technology](#Technology)
5. [Methodology](#Methodology)

## General Info

In this analysis I generate a df with the characteristics of the diamonds and their price and another df with the characteristics without the price (https://www.kaggle.com/c/diamonds-datamad0321/data). I analyse the data (type of data, descriptive statistics, sahpe, correlation...), I clean the dataset (by columns for its correlation with the price, by rows for its outliers, by null values...), I apply feature engineering (creation of columns) and application of the optimal models (gridsearch).

## Data treatment

The realization of the project is divided into up to 3 parts: 

1. Analysis: 
  - Types (Category or numerical)
  - Descriptive statistics
  - Sahpe
  - Correlation
  
2. Cleaning:
  - Columns: Correlation
  - Rows: Atypical points
  - Null values (none)

3. Feature Engineering:
  - By hand with a dictionary (map) instead of label encoder
  - Get dummies
 
4. Modelling:
  - ForestRegressor
  - RandomForestRegressor (GridSearchCV)
  
 5. Applying: 
 - Find best params and training it with all data. using it for the test.csv and saving 
 - uploading to Kaggle

## Libraries

```
pandas
matplotlib.pyplot
seaborn 
sklearn.pipeline
sklearn.preprocessing
sklearn.model_selection: train_test_split and GridSearchCV
sklearn.metrics: mean_squared_error and make_scorer
sklearn.linear_model: LinearRegression
sklearn.ensemble: IsolationForest and RandomForestRegressor

```
## Technology: 

A list of technologies used within the project:

1. [Jupyter Notebook](https://jupyter.org/) : Version 6.1.4
2. [Python](https://www.python.org/): Version 3.8

## Methodology: 

The realization of the project is divided into up to 2 parts: 

1. Preliminary analysis, cleaning and, preparing of the dataset.

* Import the csv from the files.

* Analysing:
* - Analysing:
* - Types (Category or numerical)
* - Descriptive statistics
* - Sahpe
* - Correlation

* Data cleansing and data processing:
* - Outliers: Deleting rows when more than 50% of the features are outliers.

* Feature Engineering:
* - I have tried using label encoder but I realised that it was not working propperly. Then I have apply (with map) a dictionary to the "cut" columns.
* - Get Dummies for two features "color" and "clarity".

* Saving the booth .csv.

2. Modelling.

* Import the csv from the files.

* Splitting the training df to test and compare my models

* Modelling with:
* - LinearRegression
* - RandomForestRegression
* - GridSearchCV to find the best hyperparameters
* - Training with all de dataset.

* Saving the booth .csv.

## Author

* **Bertrán Gil de Santivañes Finat** - *Initial work* - (https://github.com/Bertrangsf/5.-Diamond-Competition)
