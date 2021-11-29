# Prophet Forecast
# Time Series Forecast with Prophet

## Introduction:
This is a simple kernel in which we will forecast stock prices using Prophet. Although historical prices do not predict the future results, historical prices are being studied to provide insights into their products, with an overview of overperform or underperform of the investments.  


## A Summary about Prophet:
Facebook's research team has come up with an easier implementation of forecasting through it's new library called Prophet. According to some analysts that prophet can produce high quality forecasting data is rarely seen. This is one of the reasons why Facebook's research team came to an easily approachable way for using advanced concepts for time series forecasting and us Python users, can easily relate to this library since it uses Scikit-Learn's api (Similar to Scikit-Learn). To gain further information, please refer to  [Prophet Blog](https://research.fb.com/prophet-forecasting-at-scale/). Prophet's team main goal is to <b>to make it easier for experts and non-experts to make high quality forecasts that keep up with demand.

# Background
We'll be analyzing stock data related to Amazon (online retail stocks), Tesla ( Electric vehicles), S&P 500 for the period of July 2018 to November 2021. The main reason for selecting Amazon stock in this analysis is due to its popularity being known as one of the top pick among U.S. Internet Stocks.  According to Goldman Sachs Group Inc., Amazon is poised to outperform in 2022 as it benefits from resurgent growth in a range of markets, including e-commerce, cloud computing and advertising.  Next, in a fast-changing world Tesla has gained massive stock growth and now sports a market capitalisation of $777 billion.
  

# Part 1: Import various libraries and dependencies
Collect Investments Data Using Alpaca: AMZN, TSLA, SPY

  
 # Part 2: Data Cleaning 
Create DataFrames from CSV files and become confident using the basic commands to manipulate them
Demonstrate the ability to clean data using the DataFrame built-in commands
Manipulate data using DataFrame indexes
Describe the basic theory and calculations of returns using Pandas
Manipulate datetime data in single variable, DataFrame columns, and Series formats
Identify the calculations that can be done with datetime data
  
  
  
  
 # Part 3: Data Visualisation
 Recreate this linear plot of all the stocks' Open price
  
  
  
  
  
  
  
  Plot the Volume of stock traded each day.
  
  
 
  
  
  Interesting, looks like Amazon had a really big spike somewhere in late 2013. What was the date of this maximum trading volume for Amazon?
  
  
  
  
  
  
  
  Similarly, looks like Tesla had a really big spike somewhere in late 2013. What was the date of this maximum trading volume for Amazon?
  
  
  
  
  
 # Visualize trends through rolling statistics that smooth datasets and minimize data noise.
  
  
  
 # Define correlation and explain how to calculate it in Pandas.
  
  
  
  # Build and optimize a portfolio by factoring in risk, correlation, and returns.
  
  
  
  
  # Compare a portfolio's performance to other portfolios.
  The Open Price Time Series Visualization makes Tesla look like its always been much more valuable as a company than SPY and AMZN. In order to heighten our understanding, we 
  would need to look at the total market cap of the company, not just the stock price. Unfortunately our current data doesn't have that information of total units of stock 
  present. But what we can do as a simple calcualtion to try to represent total money traded would be to multply the Volume column by the Open price. Remember that this still 
  isn't the actual Market Cap, its just a visual representation of the total amount of money being traded around using the time series. (e.g. 100 units of stock at $10 each 
  versus 100000 units of stock at $1 each)

  Create a new column for each dataframe called "Total Traded" which is the Open Price multiplied by the Volume Traded.
  
  
