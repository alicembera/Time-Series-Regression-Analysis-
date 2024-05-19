# Regression-Project-on-Coorporation-Favorita
Corporation Favorita aims to optimize its inventory management by accurately forecasting the demand for various products across its stores in Ecuador. The goal is to ensure that each store has the right quantity of products in stock to meet customer demand while minimizing overstocking or stockouts.

## Introduction
Corporation Favorita wants to ensure that they always have the right quantity of products in stock. To do this I have decided to build a series of machine learning models to forecast the demand of products in various locations. The marketing and sales team have provided you with some data to aid this endeavor. CRISP-DM Framework for Data Science projects were used.

## Insights from data analysis
The dataset provided were train, test, stores, oil, transaction, sample_submission and holiday_events. However, the main dataset used in the analysis were the train and test datasets whiles the other supplementary datasets were useful in answering the hypothesis and the questions of interest.

## Hypothesis and Questions
The following hypothesis was stated for the regression analysis:

Null Hypothesis (Ho): Holidays do not have a significant effect on the sales. 

Alternate Hypothesis (Ha): Holidays have a significant effect on the sales.

## Questions
1. Is the train dataset complete (has all the required dates)?
2. Which dates have the lowest and highest sales for each year (excluding days the store was closed)?
3. Compare the sales for each month across the years and determine which month of which year had the highest sales.
4. Did the earthquake impact sales?
5. Are certain stores or groups of stores selling more products? (Cluster, city, state, type)
6. Are sales affected by promotions, oil prices and holidays?
7. What analysis can we get from the date and its extractable features?
8. Which product family and stores did the promotions affect.
9. What is the difference between RMSLE, RMSE, MSE (or why is the MAE greater than all of them?)
10. Does the payment of wages in the public sector on the 15th and last days of the month influence the store sales.

##  Overview
The objective is to build machine learning models that can predict unit sales for different product families at Favorita stores accurately. These models will help optimize inventory levels, improve sales forecasting accuracy, and ultimately enhance customer satisfaction by ensuring product availability.

As part of the project, the following processes were followed:
- Initial data import, cleanup, and overview.
- Exploratory Data Analysis - This provided more insight to uncover the need for more data cleaning.
- Model Development. (I performed data processing, built models, chose algorithms, chose best-performing model, etc)
- Model evaluation and comparison.

  ## Data Import, Clean-up, and Exploratory Data Analysis (EDA)
  The following libraries were imported to aid EID, analysis, and machine learning models.

## Library for EDA
- import pandas as pd.
- import numpy as np. 
- import seaborn as sns.
- %matplotlib inline.
- import matplotlib.pyplot as plt.
- import matplotlib.dates as mdates.
- from sklearn.impute import SimpleImputer.
- from pandas_profiling import ProfileReport.
- import warnings.
warnings.filterwarnings('ignore')
- Data Import and Business Understanding.

To perform an excellent analysis, a thorough business understanding was prerequisite. As a result, I loaded the datasets (train, test, transaction, oil, stores, holidays_events, and sample_submission). The train and test datasets were used in the analysis whiles the other datasets aid the EDA in answering most of the project questions where required.

## Train Data CSV

The train data csv contained the following, time series of features from 2013/01/01 to 2017/08/15. Also, the following columns were found, store_nbr, family, target sales, and on_promotion respectively.
- The store_nbr indicated the store at which the products were sold.
- The On promotion column was the total number of items promoted at a store at a given date period.
- The target sales gave the total sales for a product class at a particular store at a given date.
- The family column identified the type of product sold.

## Overview of the transaction, oil, stores, holidays_events, and sample_submission datasets

**Transaction csv**

There were three(3) columns in the transition csv. These are date, store number, and transactions

**Oil csv**

The oil csv were contained in it the date and dcoilwtico columns

**Stores csv**

The stores csv also had store number, city, state, type, and cluster as its columns

**Holiday_events csv**

This dataset had the following columns, data, type of event, locale, locale name, description and transferred.

**Sample_Submission csv**

The sample_submission had only two columns, thus, the Id and sales columns.

## Checking columns and rows of each dataset
During the EDA it was found that each of the dataset had the following shape:
- Sample_submission csv had 28512 rows and 2 columns.
- Stores csv had 54 rows and 5 columns.
- Transaction csv had 83488 and 3 columns.
- 0il csv had 1218 rows and 2 columns.
- Train csv had 3000888 rows and 6 columns.
- Test csv had 28512 rows and 5 columns.

## Machine Learning and Modeling
At this part of the project, 5models were trained and validated. These are linear regression model, XGBRegressor, ARIMA, SARIMA, Prophet models.

## Summary 
Regression is an essential statistical method employed in time-series analysis and modeling. It helps predict future trends, uncover patterns, and evaluate the effects of past events on current data. The most frequently utilized regression techniques in time-series analysis include linear regression, ARIMA, and exponential smoothing. By comprehending the benefits of applying regression in time-series analysis, data scientists can enhance their decision-making and refine their data analysis methods.

### Thank you!

Link to article on Medium: https://medium.com/@mberaalice7/time-series-regression-analysis-on-corporation-favorita-sales-5126f25c6920


### Power BI Visualizations
![PBI 1](https://github.com/alicembera/Time-Series-Regression-Analysis-/assets/160122113/a0cdc9e1-efe9-4182-92ca-7133b03c2d2a)

![PBI2](https://github.com/alicembera/Time-Series-Regression-Analysis-/assets/160122113/1267cb77-f025-499d-a4fa-cc3433971afd)

![PBI3](https://github.com/alicembera/Time-Series-Regression-Analysis-/assets/160122113/3efe5b62-5139-4158-a89f-b44b27d513fc)

![PBI4](https://github.com/alicembera/Time-Series-Regression-Analysis-/assets/160122113/6401c5ff-5cdf-4803-8d42-6881cd6a5fc3)

![PBI5](https://github.com/alicembera/Time-Series-Regression-Analysis-/assets/160122113/32fc0bb9-d50e-4397-80ab-a8e22823278a)





## Author 
Alice Mbera




  




