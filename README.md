# Prophet Forecast
# Time Series Forecast with Prophet

## Introduction:
This is a simple kernel in which we will forecast stock prices using Prophet. Although historical prices do not represent the future prices, historical prices are being studied to provide an overview and gain insights into overperform or underperform of the stock prices.  


## A Summary about Prophet:
Facebook's research team has come up with an easier implementation of forecasting through it's new library called Prophet. According to some analysts that prophet can produce high quality forecasting data. This is one of the reasons why Facebook's research team came to an easily approachable way for using advanced concepts for time series forecasting and the Python users.  For further reading, please refer to  [Prophet Blog](https://research.fb.com/prophet-forecasting-at-scale/). Prophet's team main goal is to to make it easier for experts and non-experts to make high quality forecasts that keep up with demand.

# Background
We'll be analyzing stock data related to Amazon (online retail stocks), Tesla ( Electric vehicles), S&P 500 for the period of July 2018 to November 2021. The main reason for selecting Amazon stock in this analysis is due to its popularity being known as one of the top pick among U.S. Internet Stocks.  According to Goldman Sachs Group Inc., Amazon is poised to outperform in 2022 as it benefits from resurgent growth in a range of markets, including e-commerce, cloud computing and advertising.  Next, in a fast-changing world Tesla has gained massive stock growth and now sports a market capitalisation of $777 billion.
  

# Part 1: Import various libraries and dependencies
Collect Investments Data Using Alpaca: AMZN, TSLA, SPY

  
 # Part 2: Data Cleaning 
Create DataFrames from CSV files and use basic commands to manipulate them
Clean data using the DataFrame built-in commands
Manipulate data using DataFrame indexes
Describe the basic theory and calculations of returns using Pandas
Manipulate datetime data in single variable, DataFrame columns, and Series formats

  
  
  
  
 # Part 3: Data Visualisation
 AMZN stock price
 ## ![Amazon Share price](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20Share%20Prices.JPG?raw=true)
  
 Amazon shares bottomed out at around $1,600 in mid-March as the stock market plunged amid widespread business shutdowns due to the coronavirus pandemic. The stock has since roared back from its March low, closing above $3,000 per share for the first time on July 6. There are several reasons to explain the stock’s “meteoric rise,”.  According to analyst Sucharita Kodali, it is one of the most diversified companies out there.  It just defies gravity.   It isn’t just an e-commerce business that has prospered during COVID-19. Amazon Web Services continues to power much of the internet, even having posted faster growth than the company in its entirety during the second quarter. And Amazon’s video streaming service has been one of the most added by American households. Investors have rewarded the company’s growth by nearly doubling share prices from their late-2019 levels.
 
  

  Volume Traded and Interpretation for AMZN
  Plot AMZN Trading Volume - 1month, 6months, YTD, 1 year, all
  ## ![AMZ Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/AMZN%20Trading%20Volume.jpg)
  
  
  
  Amazon shares surge in April 2020 and the highest trading volume recorded. 
  
  
  ## ![AMZ Highest Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/AMZN%20Highest%20Traded%20Volume.JPG)
  This is due to the pandemic hit in the early 2020. According to the Fortune (2021), when the pandemic hit last year, most of corporate America got caught flat-footed. More than 200,000 businesses, including many restaurants and retailers, permanently shuttered owing to COVID-19. Amazon, meanwhile kept on growing , bcoming much more massive. Even in the face of supply chain slowdowns, a tight labor market, and COVID-19 outbreaks in its facilities, Amazon has become the go-to source over the past two years for people around the globe looking for everything from essential goods like laundry detergent and toilet paper to work-from-home necessities such as soundproof headphones.



# 
  
  TSLA stock price
 ## ![Tesla Share price](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Tesla%20Share%20Prices.JPG?raw=true) 

Tesla operates through two segments: Automotive, and Energy generation and storage. It occupies a market-leading position in the electric car industry and is pioneering much of the road towards self-driving vehicles – and with many politicians ostensibly backing a green recovery after the coronavirus pandemic, the value of cleaner technology looks ever greater.  Having said, much of the 2020 share price rise has also been ascribed to a scramble by non-professional investors shorting on the Tesla name. More than 450,000 small investors have bought Tesla shares through the commission-free Robinhood trading platform in the US. On one single day in July there were 50,000 new Tesla investors, according to The Guardian, 2020.  Analysts from Morgan Stanley warned that Tesla is “grossly overvalued” and that the share price would plunge.
  
  
  
  Volume Traded and Interpretation for TSLA
  Plot TSLA Trading Volume - 1month, 6months, YTD, 1 year,All
  ## ![TSLA Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Tesla%20Trading%20Volume.JPG)
  
  
  
  
  Tesla shares surge in August 2020 and the highest trading volume recorded.
  
  
  ## ![TSLA Highest Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/TSLA%20Highest%20Traded%20Volume.JPG)
  
  Tesla shares continued to rise after in particular it overtook Toyota as the world's most valuable company in July.  The share price was further fuelled by the announcement of a 5 for 1 split on August 28, in which the share price reset from $2,230 to a far more accessible $446 - which technically should not affect the company valuation but makes the price for each individual share more attainable for small investors.  Prices surged by 13% on the same day, resulting in the comapny's stock price appreciated nbearly 500% between January 1 and August 31 2020, according to Nasdaq.
  On the other hand, there's a mixed bag of news when Tesla encountered some setbacks in China. With the rapid increasing competition in the EV market, along with Chinese electric vehicle maker NIO and the European carmakers, Tesla's China registation has dropped in July, but investors were hoping for continue momentum.
  
  
  
  # Market Cap
  The Open Price Time Series Visualization makes Tesla shares look more attractive. But to really understand this we would need to look at the total market cap of the company, not just the stock price. Unfortunately our current data doesn't have that information of total units of stock present. But what we can do as a simple calcualtion to try to represent total money traded would be to multply the Volume column by the Open price. Remember that this still isn't the actual Market Cap, its just a visual representation of the total amount of money being traded around using the time series. (e.g. 100 units of stock at $10 each versus 100000 units of stock at $1 each)
  
  
  
  

 # Part 4 : Correlation and Scatter Matrix
 
 ## ![Scatter Plot Dashboard](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20stocks%20-%20Panel%20Dashboard.JPG)
 
 
  
 
 # Part 5: Volatity
  ## ![Combined Stocks 21 Days Deviation](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%2021%20Days%20Standard%20Deviation.JPG)
  
  
  ## ![Combined Stocks 21 Days Rolling](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%2021%20Days%20rolling%20mean.JPG)
  
  
  # Part 6: Risk Analysis
  
 ## ![Combined Stocks Risk Analysis](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Risk%20Analysis.JPG)
 
 
  # Part 7 : Cumulative Return
  ## ![Combined Stocks Cumulative Returns](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Cumulative%20Returns.JPG)
  
