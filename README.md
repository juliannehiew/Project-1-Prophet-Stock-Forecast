# Amazon Prophet Forecast
# Time Series Forecast with Prophet

## Introduction:
This is a simple kernel in which we will forecast stock prices using Prophet. Although historical prices do not represent the future prices, interpreting historical prices can enhance the insights into overperform or underperform, and identify the level of volatility of the stock prices discussed in this analysis.  


## A Summary about Prophet:
Facebook's research team has come up with an easier implementation of forecasting through it's new library called Prophet. According to some analysts that prophet can produce high quality forecasting data. This is one of the reasons why Facebook's research team came to an easily approachable way for using advanced concepts for time series forecasting and the Python users.  For further reading, please refer to  [Prophet Blog](https://research.fb.com/prophet-forecasting-at-scale/). Prophet's team main goal is to make it easier for experts and non-experts to make high quality forecasts that keep up with demand.

# Background
Three stock data related to Amazon (online retail stocks), Tesla ( Electric vehicles), S&P 500 for the period of July 2018 to November 2021 will be analysed in this stock analysis. The main reason for selecting Amazon stock is due to its popularity being known as one of the top pick among U.S. Internet Stocks.  According to Goldman Sachs Group Inc., Amazon is poised to outperform in 2022 as it benefits from resurgent growth in a range of markets, including e-commerce, cloud computing and advertising.  Next, in a fast-changing world, Tesla that achieved a massive stock growth has sports a market capitalisation of $1.137 Trillion, resulting in the world's 6th most valuable company is selected for comparison purposes.  Thirdly, S&P 500 is used as a benchmark in this analysis due to its central advantage being the wide market breadth of the large-cap companies included in the index. The index can provide a broad view of the economic health of the United States.

In addition to its broad scope, another advantage of the S&P 500 is that components of the index are updated on a quarterly basis. A committee determines which companies to include in the index. The factors considered include a market capitalization in excess of $6.1 billion, a public float of at least 50 percent, headquarters in the U.S., adequate liquidity and financial viability.
  

# Part 1: Import various libraries and dependencies
Collect Investments Data Using Alpaca: AMZN, TSLA, SPY

  
 # Part 2: Data Cleaning 
Create DataFrames from CSV files and use basic commands to manipulate the data.
Clean data using the DataFrame built-in commands.
Manipulate data using DataFrame indexes.
Describe the basic theory and calculations of returns using Pandas.
Manipulate datetime data in single variable, DataFrame columns, and Series formats.

  
  
  
  
 # Part 3: Data Visualisation
 AMZN stock price
 ## ![Amazon Share price](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20Share%20Prices.JPG?raw=true)
  
 Amazon shares bottomed out at around $1,600 in mid-March as the stock market plunged amid widespread business shutdowns due to the coronavirus pandemic. The stock has since roared back from its March low, closing above $3,000 per share for the first time on July 6. There are several reasons to explain the stock’s “meteoric rise,”.  According to analyst Sucharita Kodali, it is one of the most diversified companies out there.  It just defies gravity.   It isn’t just an e-commerce business that has prospered during COVID-19. Amazon Web Services continues to power much of the internet, even having posted faster growth than the company in its entirety during the second quarter. And Amazon’s video streaming service has been one of the most added by American households. Investors have rewarded the company’s growth by nearly doubling share prices from their late-2019 levels.
 
  

  Volume Traded and Interpretation 
  AMZN Trading Volume - 1month, 6months, YTD, 1 year, all
  ## ![AMZ Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/AMZN%20Trading%20Volume.jpg)
  
  
  
  Amazon shares surge in April 2020 and the highest trading volume recorded. 
  
  
  ## ![AMZ Highest Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/AMZN%20Highest%20Traded%20Volume.JPG)
  This is due to the pandemic hit in the early 2020. According to the Fortune (2021), when the pandemic hit last year, most of corporate America got caught flat-footed. More than 200,000 businesses, including many restaurants and retailers, permanently shuttered owing to COVID-19. Amazon, meanwhile kept on growing , bcoming much more massive. Even in the face of supply chain slowdowns, a tight labor market, and COVID-19 outbreaks in its facilities, Amazon has become the go-to source over the past two years for people around the globe looking for everything from essential goods like laundry detergent and toilet paper to work-from-home necessities such as soundproof headphones.



# 
  
  TSLA stock price
 ## ![Tesla Share price](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Tesla%20Share%20Prices.JPG?raw=true) 

Meanwhile, Tesla operates through two segments: Automotive, and Energy generation and storage. It occupies a market-leading position in the electric car industry and is pioneering much of the road towards self-driving vehicles – and with many politicians ostensibly backing a green recovery after the coronavirus pandemic, the value of cleaner technology looks ever greater.  Having said, much of the 2020 share price rise has also been ascribed to a scramble by non-professional investors shorting on the Tesla name. More than 450,000 small investors have bought Tesla shares through the commission-free Robinhood trading platform in the US. On one single day in July there were 50,000 new Tesla investors, according to The Guardian, 2020.  Analysts from Morgan Stanley warned that Tesla is “grossly overvalued” and that the share price would plunge.
  
  
  
  Volume Traded and Interpretation 
  TSLA Trading Volume - 1month, 6months, YTD, 1 year, all
  ## ![TSLA Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Tesla%20Trading%20Volume.JPG)
  
  
  
  
  Tesla shares surge in August 2020 and the highest trading volume recorded.
  
  
  ## ![TSLA Highest Trading Volume](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/TSLA%20Highest%20Traded%20Volume.JPG)
  
  Tesla shares continued to rise after in particular it overtook Toyota as the world's most valuable company in July.  The share price was further fuelled by the announcement of a 5 for 1 split on August 28, in which the share price reset from $2,230 to a far more accessible $446 - which technically should not affect the company valuation but makes the price for each individual share more attainable for small investors.  Prices surged by 13% on the same day, resulting in the company's stock price appreciated nearly 500% between January 1 and August 31 2020, according to Nasdaq.
  On the other hand, there's a mixed bag of news when Tesla encountered some setbacks in China. With the rapid increasing competition in the EV market, along with Chinese electric vehicle maker NIO and the European carmakers, Tesla's China registation has dropped in July 2020, but investors were hoping for continue momentum.
  Following this, Tesla dreams about making it into S&P 500 Index is about to become reality. Unfortunately, in September 2020 at the very last the firm is passed over for entry, and a lot of people are very disappointed. When news lands that it wouldn’t be included, the share price plummets 21.06% in the worst single day loss in the company’s history.  However, it’s always darkest before the dawn. The next day proved much more promising, perhaps as investors began to suspect shares had been oversold. Prices steadily rose, jumping around 11% on September 9. Even so, after its ground-breaking August, prices dropped from $2,510.70 on September 1 to $1,651.05 at closing on September 8.
  
  
  
  # Market Cap
  The Open Price Time Series Visualization makes Tesla shares look more attractive. Notwithstanding, we would need to look at the total market cap of the company, not just the stock price. Unfortunately our current data doesn't have sufficient information of total units of stock present. As such a simple calcualtion to try to represent total money traded would be applied to multply the Volume column by the Open price. A reminder that this still isn't the actual Market Cap, its just a visual representation of the total amount of money being traded around using the time series. (e.g. 100 units of stock at $10 each versus 100000 units of stock at $1 each)
  
  ## ![Market - AMZN](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/AMZN%20Total%20Traded.JPG)
  
  
  ## ![Market - TSLA](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/TSLA%20Total%20Traded.JPG)
  

 # Part 4 : Visualize trends through rolling statistics that smooth datasets and minimize data noise.
 
 Correlation and Scatter Matrix
 
 ## ![Scatter Plot Dashboard](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20stocks%20-%20Panel%20Dashboard.JPG)
 
 The scatter plot in this dashboard is a special type of graph designed to identify the relationship between two or more variables. With regression analysis, we visually inspect the data to see whether X and Y are linearly related. With reference to these plots, the graph isn't a straight line, the relationship between AMZN and TSLA is proven to be non-linear because they are in different industries.  Similarly, non-linear relationship is identified between AMZN and SPY, or TSLA and SPY.  In short, there's no meaningful correlation in these 3 stocks.
  
  
  Rolling Statistics - AMZN
 ## ![Rolling Statistics - AMZN](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20-%20Rolling%20Statitics%2030%20Days.JPG)
 
 
 ## ![Density Plot - AMZN](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20-%20Density%20Daily%2030%Returns.JPG)
 

 
  Standard Deviation - AMZN
 ## ![Standard Deviation - AMZN](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20-%20Standard%20Deviation%2030%20Days.JPG)
 
 Standard deviation is a useful tool in investing and trading strategies as it helps measure market and security volatility and predicts performance trends.  Despite a lower standard deviation represents a stable blue-chip stock, it isn't necessarily preferable. It all depends on the investments and the investor's willingness to assume risk. When dealing with the amount of deviation in their portfolios, investors should consider their tolerance for volatility and their overall investment objectives. More aggressive investors may be comfortable with an investment strategy that opts for vehicles with higher-than-average volatility, while more conservative investors may not.  
 
 With reference to the chart, TSLA has a high standard deviation particularly during May and September 2020.  As such it is regarded as a volatile stock.  One of the factors contributing to the soaring prices during April/May 2020 is driven by the positive news on the expansion of Tesla's Shanghai factory.  Following this, the analysts have upgraded the stock price, which led to a price surge as a result. 
 
 Having said, the drawback of standard deviation assumes a normal distribution and calculates all uncertainty as risk. 
  
  # Part 5: Moving Averages
  
  Moving Averages - AMZN
   ## ![Moving Averages - AMZN](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20-%20Moving%20Averages.JPG)
   
   Moving Averages - TSLA
   
   ## ![Moving Averages - TSLA](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/TSLA%20-%20Moving%20Averages.JPG)
   
   
   Moving averages are an important analytical tool used to identify current price trends and the potential for a change in an established trend. The simplest use of a Simple Moving Average in technical analysis is using it to quickly identify if a security is in an uptrend or downtrend. Another popular, albeit slightly more complex, analytical use is to compare a pair of simple moving averages with each covering different time frames. If a shorter-term simple moving average is above a longer-term average, an uptrend is expected. On the other hand, if the long-term average is above a shorter-term average then a downtrend might be the expected outcome.
  
 
 # Part 6: Volatity
 Which stock is the most volatile?
 
 ## ![Combined Stocks Daily Return](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Daily%20Returns.JPG)
 
 
 ## ![Combined Stocks Density of Daily Returns](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Standard%20Deviation.JPG)
 
 
  ## ![Combined Stocks 21 Days Deviation](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%2021%20Days%20Standard%20Deviation.JPG)
  
  
  ## ![Combined Stocks 21 Days Rolling](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%2021%20Days%20rolling%20mean.JPG)
  
  
  These datasets are considered noisy, displaying large momentums of each stocks, especially TSLA.  The sharp plunge of TSLA stocks on end of August 2020 is closely associated with the drop in registrations of EV in China as mentioned above.   
  
  
  
  
  
  
  # Part 7: Comparision of Stock Performance
  
 One of the most commonly used and talked about risk measures in investing is the Sharpe Ratio. Sharpe Ratio tells an analyst the return per unit of risk. In other words, how much extra return you will receive per unit of risk that you take on.  Any Sharpe Ratio above 1.00 generally means the portfolio or stock is acceptable to hold because you are receiving an excess return per unit of risk. Anything above 2.00 or 3.00 is considered very good. The opposite can be said for anything with a Sharpe Ratio below 1.00, where it may worry an investor that they are putting their money into a more risky asset.
 
 
 
 ## ![Combined Stocks Risk Analysis](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Risk%20Analysis.JPG)
 
 In comparision of the three stocks, TSLA has the most outliers; what this suggests is that during the period being considered, same stock 'over-perform' and as well 'under-perform' in relation to where the bulk of the rest data values. The enclosed area where signifies 50% of the data is resident lies within the box. In respect to the box plot, SPY has the narrowest box that indicates the interquartile range of +-25% from the mean is more condensed than the interquartile range of +-25% from the mean of AMZN. Although this spread of the data points of Amazon is smaller than the spread of the data points of SPY.
 
 
  # Part 8 : Cumulative Return
  ## ![Combined Stocks Cumulative Returns](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Combined%20Stocks%20-%20Cumulative%20Returns.JPG)
  
A cumulative return on an investment is the aggregate amount that the investment has gained or lost over time, independent of the amount of time involved. The cumulative return is expressed as a percentage in the graph.  The above results implied that TSLA has the best cumulative return as compared to AMZN and SPY. 



# Part 9: AMAZON PROPHET FORECAST ANALYSIS STARTS

Amazon Stock Price Forecast
## ![Amazon Stock Price Forecast](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Amazon%20Stock%20Price%20Forecast.JPG)

## ![Monthly Prediction](https://github.com/juliannehiew/Project-1-Prophet-Stock-Forecast/blob/main/Monthly%20Prediction.JPG)


# Summary

Overall the outcomes of AMZN, TSLA, and SPY continue to show strength and eventually pushed the major averages higher. 
The key takeaways are Amazon has grown to be one of the most successful companies in the world, grabbing the market share not only in retail but cloud computing, media, and entertainment. Its profound advances in data, analytics, and digital technology, has contributed to its market cap of $1.806 Trillion.  Amazon has confirmed the continuing strong demand for cloud services reporting +39% increase in revenue year-on-year and continues to lead the fast-growing cloud infrastructure-as-a-service market with 41% global market share. This ongoing strong demand for public cloud is driven by accelerating digital transformation across the broad corporate world, which underpins corporate spending on software and cloud solutions across industries. This is increasingly relevant to companies with rising cost structures, which are now investing in cost rationalisation initiatives through digital transformation. 

This drives the stock price further uptrend, especially when the investors move into tech stocks broadly as U.S. Treasury yields took a dip of roughly 2 basis points as of writing. Amazon has gained 4% as its first cashierless coffeeshop, which it partnered on with Starbucks, opened in New York. It also got a lift from continued positive momentum in retail, particularly in digital - Amazon’s Services, notably AWS which is growing rapidly and generate considerable profits.   

Despite its success, the company remains open to competitors as well as razor-thin profit margins.

The company's stock has a beta of around 1.3 and trailing Price/Earning ration of 138x, considering it as a highly specualtive investment fueled by anticipation of even greater growth ahead (Investopedia, 2020).
 






Disclaimer: This material contains general market commentary.  It does not constitute investment research or personal advice. The opinions expressed are based on exploratory data analysis and predictive data analysis.
