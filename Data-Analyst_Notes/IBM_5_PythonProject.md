
# PYTHON PROJECT FOR DATA SCIENCE #

### SUMMARY ###

In this module, you will demonstrate your skills in Python - the language of choice for Data Science and Data Analysis. You will apply Python fundamentals, Python data structures, and work with data in Python. By working on a real project, you will model a Data Scientist or Data Analyst's role, and build a dashboard using Python and popular Python libraries using Jupyter notebook.

Learning Objectives

    Perform webscraping in Python to obtain data.
    Extract data by using a Python library.


## WELCOME ##

Welcome to this Python Project!  

This mini-course is intended to be a follow-on to the Python for Data Science, AI and Development

 course for you to demonstrate basic Python skills that you have acquired in that course.

In this mini-course you will be assuming the role of a Data Scientist / Data Analyst. In this role you will be given a scenario and data to begin your Python project. During this process you will perform specific tasks such as extracting data, web scraping, visualizing data, and creating a dashboard. You will then submit your Python notebook and screenshots for your peers to review and evaluate your work.

To be successful in completing this project, you should have already completed the Python for Data Science, AI and Development course or have equivalent skills for working with Data and Python.



## ANALYZING STOCK PERFORMANCE AND BUILDING A DASHBOARD ##

### PROJECT OVERVIEW

For this project, you will assume the role of a Data Scientist / Data Analyst working for a new startup investment firm that helps customers invest their money in stocks. Your job is to extract financial data like historical share price and quarterly revenue reportings from various sources using Python libraries and webscraping on popular stocks. After collecting this data you will visualize it in a dashboard to identify patterns or trends. The stocks we will work with are Tesla, Amazon, AMD, and GameStop.

Dashboard Analytics Displayed

A dashboard often provides a view of key performance indicators in a clear way. Analyzing a data set and extracting key performance indicators will be practiced. Prompts will be used to support learning in accessing and displaying data in dashboards. Learning how to display key performance indicators on a dashboard will be included in this assignment. We will be using Plotly in this course for data visualization and is not a requirement to take this course.

In the Python for Data Science, AI and Development course you utilized Skills Network Labs for hands-on labs.

For this project you will use Skills Network Labs and Watson Studio. Skills Network Labs is a sandbox environment for learning and completing labs in courses. Whereas Watson Studio, a component of IBM Cloud Pak for Data, is a suite of tools and a collaborative environment for data scientists, data analysts, AI and machine learning engineers and domain experts to develop and deploy your projects.

Review criteria

There are two hands-on labs on Extracting Stock Data and one assignment to complete. You will be judged by completing two quizzes and one peer review assignment. The quizzes will test you based on the output of the hands-on labs. In the peer review assignment you will share and take screen shots of the outcomes of your assignment.


### STOCK SHARES

A company's stock share is a piece of the company; more precisely:

A stock (also known as equity) is a security that represents the ownership of a fraction of a corporation
. This entitles the owner of the stock to a proportion of the corporation's assets and profits equal to how much stock they own. Units of stock are called "shares."

An investor can buy a stock and sell it later. If the stock price increases, the investor profits, If it decreases,
the investor with incur a loss.  Determining the stock price is complex; it depends on the number of outstanding shares, the size of the company's future profits, and much more. People trade stocks throughout the day. The stock ticker is a report of the price of a certain stock, updated continuously throughout the trading session by the various stock market exchanges. In this lab, you will use the  y-finance API to obtain the stock ticker and extract information about the stock. You will then be asked questions about your results.  


### FINANCE LIBRARY

The yfinance is a Python library that provides a user-friendly interface for downloading historical market data from Yahoo Finance. It allows you to get historical stock prices, dividends, and other financial data for stocks, Exchange-Traded Funds (ETFs), and other securities.

This example shows code on how to use yfinance to download historical stock prices:

    1    import yfinance as yf
    2
    3    # Download historical data for a stock
    4    msft = yf.Ticker("MSFT")
    5    msft_data = msft.history(period="max")
    6
    7    # Display the downloaded data
    8    msft_data.head()


In the above code:

    First, import the yfinance library using the alias yf.
    Then, create a Ticker object for the Microsoft stock (“MSFT”).
    Use the history method of the Ticker object to download the historical data for the stock. The period parameter of the history method specifies the time period for which we want to download the data. In this example, set it to max to download the maximum amount of available historical data.

Here are some of the possible values for the period parameter and what they represent:

    period="1d": Download 1 day of historical data.
    period="5d": Download 5 days of historical data.
    period="1mo": Download 1 month of historical data.
    period="3mo": Download 3 months of historical data.
    period="6mo": Download 6 months of historical data.
    period="1y": Download 1 year of historical data.
    period="2y": Download 2 years of historical data.
    period="5y": Download 5 years of historical data.
    period="10y": Download 10 years of historical data.
    period="ytd": Download historical data since the beginning of the current year.
    period="max": Download all available historical data.

Finally, we print the downloaded data using the head function. This will display a Pandas DataFrame containing the historical stock prices and other financial data for Microsoft.



### GAMESTOP STOCK VS TESLA

Determining the price of a stock is complex; it depends on the number of outstanding shares, the size of the company's future profits, and much more.  An essential factor is the company's profit and growth of profits; if the company's profit is increasing, the stock price should increase.  If you suspect the company's profit increases, you should buy the stock as the stock should increase, But what happens if you think the stock price will decrease. 

Short selling is how you make money if the stock decreases. An investor borrows a stock, sells the stock, and then repurchases it to return it to the lender.  Typically stocks fall faster than they rise, so you can make a profit more quickly. Usually, experienced investors such as hedge funds partake in short selling. One problem is if the stock price increases, the investor can lose money.

Sometimes short sellers get it wrong; for example, Tesla.  A few years ago, many short sellers targeted Tesla. Then Tesla started becoming profitable, and profits were increasing; thus, the company stock went up. This was based on the companies performance, so the stock should continue to rise, and the short seller should sell the stock.  Recently shorted stocks can increase for reasons that are not based on fundamentals; this is less sustainable. 

Individual investors using the forum on the Reddit online community named WallStreetBets, started buying into shares of GameStop, a video and computer-game retailer losing money. The influx of demand caused GameStop shares to soar.  All this produced billions of dollars in losses for hedge funds who had sold the stock short. [ 1
] GameStop's share price should fall eventually, so the Hedge funds should hold on to the short positions. As a data scientist working for a hedge fund, you will extract the profit data for Tesla and GameStop and build a dashboard to compare the price of the stock vs the profit for the hedge fund.



## EXAM ##

At this point please ensure you have completed the two previous yfinance and web scraping labs. In this assignment you will upload screenshots of your code and results. You will also be reviewing the submission for one of your peers and grading their work.

As a data scientist working for an investment firm, you will extract the revenue data for Tesla and GameStop and build a dashboard to compare the price of the stock vs the revenue. 
Review criteria

Full Points: Working code that yields correct results

You will be graded on the dashboards displaying the specified data and the screenshots you took during the final project lab questions. There are 12 possible points for this assignment. Here is the breakdown:

Question 1 - Extracting Tesla Stock Data Using yfinance - 2 Points
Question 2 - Extracting Tesla Revenue Data Using Webscraping - 1 Points
Question 3 - Extracting GameStop Stock Data Using yfinance - 2 Points
Question 4 - Extracting GameStop Revenue Data Using Webscraping - 1 Points
Question 5 - Tesla Stock and Revenue Dashboard - 2 Points
Question 6 - GameStop Stock and Revenue Dashboard- 2 Points
Question 7 - Sharing your Assignment Notebook - 2 Points

For each problem points will be awarded as follows:

Full Points: Working code that yields correct results
Partial Points: Partially correct code or results
No Points: Did not attempt the problem or did not upload any solution
Example Submissions

Here are some examples of a submission clearly showing both the Code and its Results/Output when executed from a Jupyter Notebook.

>>>>> PNG "EXAM QUESTION"
