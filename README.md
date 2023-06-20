PHASE 4 PROJECT :REAL ESTATE TIME SERIES ANALYSIS.
1). Business Understanding
Real estate investment is a lucrative and dynamic industry that requires careful analysis and decision-making. The fictional real estate investment firm is seeking guidance on identifying the top 5 zip codes for investment opportunities. To address this question, historical data from Zillow Research is utilized.

i) Background:
Real estate investment is a lucrative and dynamic industry that requires careful analysis and decision-making. The fictional real estate investment firm is seeking guidance on identifying the top 5 zip codes for investment opportunities. To address this question, historical data from Zillow Research is utilized. The dataset contains information on various attributes, including RegionID, RegionName, City, State, Metro, SizeRank, CountyName, and value (real estate prices).

ii). Main Objective:
The main objective of this project is to identify the top 5 zip codes that offer the best investment potential in terms of real estate prices. By analyzing historical trends and patterns, the project aims to provide actionable insights to the investment firm, enabling them to make informed decisions on where to allocate their resources.

Specific Objectives:
Analyze Historical Data: The project involves analyzing the historical data of real estate prices across different zip codes. This includes understanding the trends, patterns, and fluctuations in property values over time.

Identify Promising Zip Codes: Using the analysis of historical data, the project aims to identify the zip codes that have shown consistent growth, stability, or potential for future appreciation. These zip codes are considered the most favorable for investment.

Consider Location Factors: In addition to the historical performance, the project also takes into account location-specific factors such as city, state, and metro. This information helps assess the overall desirability and attractiveness of the investment opportunities.

Evaluate Market SizeRank: The SizeRank attribute provides insights into the relative size and competitiveness of the real estate market in each zip code. This factor helps gauge the potential opportunities and risks associated with investing in a particular area.

2). Data Understanding
The dataset contains information on various attributes, including RegionID, RegionName, City, State, Metro, SizeRank, CountyName, and value (real estate prices). Our dataset is the Zillow Housing Dataset which was sourced from Zillow Research Page.

Column Name Description
RegionID -This is unique Id for the Regions
SizeRank -This is the ranking done based on the size of the region
RegionName - This field contains the zip code of the region.
RegionType- Type of region is Zip.
StateName - State
City - This column provide the specific City Name of Housing Data
Metro - This provide the name of the metro city around that region
County Name - This is the county name for that region
Months Column - These columns contains the prices of region for every month
In order to understand how our dataset looks like lets get a preview of this data by loading it.

3). Data Preparation
This is to make the data in a format that is good to feed to our model.It involves the following series of steps:

Cleaning the data

Checking for and dealing with missing values

Reshaping our dataset from wide to long format

4). Exploratory Data Analysis
This is basically trying to figure out more about our data , its behaviours and patterns This involves the following :

Grouping the data by month.

Read Me monthly Eda

Group the data yearly .

Eda Yearly plot

Grouping per quarter and plotting .

quarterly plot

Grouping per decade
Eda per decade

Finding the top 5 Best regions

Here we seek to find the five best regions by uing the return of investment, where high returns show the best regions. Below is a plot of our findings

ROI

Checking for trends and seasonality Here we seek to find the relevant trends in the dataset , based on the best regions, below is our plots

Line plot

Checking for the rolling statistics
Performing Dullers test.
Checking for stationarity
Detrending our dataset
Deseasonalizing our dataset
Performing Seasonal decomposition
5). Modelling
This is now creating various models to forecast our data . we created the following models :
ARIMA modelels
SARIMAX models.
PROPHET models.
First weplot the auto-correlation plots , then we do the modelling.
Arima Models
We created an Arima model, below is the statistical results.
Arima
Sarimax Models
Below is the statistical result using the Sarimax models.
Sarimax
Below is a plot of the actual and predicted values of our Sarimax model with a 1.94 RMSE

Sarimax

** Prophet Models** We used this model to forecast and predict values, below are some of our predicted values (Note: The yhat means the predicted values)

Prophet model
7). Summary
After performing time series analysis on the 10 zip codes and forecasting total returns for up to three years, we reccomend the company to invest in the following 3 zipcodes:

81611 - Location: Aspen, CO (R.O.I - 132.378817)

10021 - Location: New York, NY (R.O.I - 111.795552)

34102 - Location: Naples, FL (R.O.I - 7.605307)

As for the other 6 zip codes, they are not fit for investement given the negative returns.

Colab paid products - Cancel contracts here
