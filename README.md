# hw_m7_etf_analysis

This file analyzes a hypothetical etf portfolio consisting of 4 stocks using SQL, Python, and the Voila library. The data for each stock is contained in an accompanying .db file.

It first queries the .db file using SQL to pull all data on PYPL and chart its daily returns:

![PYPL Daily Returns](https://github.com/JunTheRewels/hw_m7_etf_analysis/etf_analyzer_files/images/1.png)

and its cumulative returns:

![PYPL Cumulative Returns](https://github.com/JunTheRewels/hw_m7_etf_analysis/etf_analyzer_files/images/2.png)

Next it optimizes the previous query by selecting only instances of "close" greater than 200, and then listing them in descending order and limiting to 10 entries to get the top 10 close prices (all of which presented near the end of the timeline):

![PYPL Top 10 Close Prices](https://github.com/JunTheRewels/hw_m7_etf_analysis/etf_analyzer_files/images/3.png)

Then the report analyzes the etf portfolio as a whole by using a SQL inner join to merge each of the 4 tables on the date column. The aggregated data is then used to provide the daily, annualized, and cumulative returns, respectively. It then plots the cumulative returns of the portfolio:

![ETF Portfolio Cumulative Returns](https://github.com/JunTheRewels/hw_m7_etf_analysis/etf_analyzer_files/images/4.png)

Finally this file is used to generate a webpage using voila:

![File as Webpage](https://github.com/JunTheRewels/hw_m7_etf_analysis/etf_analyzer_files/images/etf_analyzer_webpage.mp4)