﻿# StockMarketAnalysisAndPrediction (Time-series Analysis and Stock Price Forecast Modeling)
## Introduction
In this project, we’ll walk through the steps of time-series forecasting using different deep learning models.

- We’ll first look at the project and describe the data that we’ll use.

- Then we’ll cover the data wrangling and preprocessing steps. Although those steps do not relate directly to time series forecasting, they are crucial steps in any machine learning project.

We’ll then focus on the modeling steps, where we’ll try a set of learning models to uncover the best performer.
## Nasdaq, S&P 500, NYSE: What Does It All Mean?
Nasdaq, S&P 500, and NYSE are all well-known stock market indices and exchanges that play significant roles in the financial industry. Here's a brief explanation of each:

#### Nasdaq : 
Nasdaq stands for the National Association of Securities Dealers Automated Quotations. Nasdaq is known for its focus on technology-driven companies. Many prominent technology companies, such as Apple, Microsoft, and Amazon, are listed on the Nasdaq exchange.

#### S&P 500 : 
The S&P 500, short for Standard & Poor's 500, is a stock market index that measures the performance of 500 large publicly traded companies in the United States. It is considered a benchmark for the overall performance of the U.S. stock market. It is widely followed by investors, financial professionals, and analysts as an indicator of the health and direction of the U.S. stock market.

#### NYSE: 
NYSE stands for the New York Stock Exchange, which is one of the world's largest and oldest stock exchanges. It is located on Wall Street in New York City. The NYSE provides a platform for buying and selling various types of securities, including stocks, bonds, exchange-traded funds (ETFs).The NYSE has a long history and is known for its iconic trading floor, where traders conduct face-to-face transactions.

Each of these entities plays a crucial role in the global financial markets and serves as a vital source of investment opportunities and market insights.
We are going to use NASDAQ: American Airlines Group Inc. Common Stock (AAL),the dataset contains a total of Seven columns, listed below.

- **Date:** the period when discussing the open, high, low, close, and volume (OHLCV) of a securities price.
- **Volume:** the total number of shares traded in a security period
- **High:** the highest price at which a stock is traded during a period
- **Low:** the lowest price at which a stock is traded during a period
- **Open:** tells the price at which a stock started trading when the market opened on a particular day
- **Closing Price:** the price traders agreed on after all the action throughout the day, and
- **Adjusted Close:** While the closing price simply refers to the cost of shares at the end of the day, the adjusted closing price takes dividends, stock splits, and new stock offerings into account.
The main target is the Closing Price, as it represents the last price at which a stock trades during a regular trading session.

Now that we have a general understanding of the problem and the dataset, let’s define the objective of this project and the steps we’ll take to achieve it.
## Project Objective & Workflow 
The objective of this notebook is to create a model that can forecast the next month of Close price. here are the steps that need to be done:

### Data wrangling and preprocessing 
This step is optional. It is not directly linked to time series forecasting, but it is an important step in any machine learning project.
- **Handle Mising Values:** 
Calculate the number of missing values & Impute the missing values.
- **Handling Categorical Values:** 
Express each variable as a numerical value (all data is originally stored as strings).
- Resample the data by month.
### Feature engineering
- Identify any seasonality (Yearly,Monthly)
- Split the DateTime object into Month and Year columns.
- Scale the data
### Split the data
Make a 70:20:10 split to create training, validation, and test sets.
### Prepare for deep learning modeling
- Implement the DataWindow class.
- Define the compile_and_fit function.
- Create a dictionary of column indices and column names.
### Model with deep learning

**1.Train two baseline model.**

**2.Train a linear model.** 

**3.Train a deep neural network.** 

**4.Train an LSTM.**

**5.Train a CNN**.

**6.Train a combination of LSTM and CNN.**

**7.Train an autoregressive LSTM.** 

Select the best-performing model.
