# Overview

## Impact of Bitcoin Market Sentiment on Trader Performance and Risk Behavior

This project analyzes the relationship between **Bitcoin market sentiment** and **trader behavior on Hyperliquid**. By combining the **Fear & Greed Index** with historical trading data, the study investigates how different market sentiment regimes influence profitability, trading activity, position sizing, and trader decision-making.

The analysis merges daily sentiment data (Fear, Extreme Fear, Greed, and Extreme Greed) with trade-level execution records to evaluate whether traders behave differently under varying market conditions and whether sentiment can help explain trading outcomes.

### Objectives

* Analyze trader profitability across different sentiment regimes.
* Compare trading activity during Fear and Greed periods.
* Evaluate the relationship between trade size, fees, and profitability.
* Identify behavioral patterns among successful and unsuccessful traders.
* Segment traders into distinct groups using clustering techniques.
* Build a machine learning model to predict profitable trades using market sentiment and trade characteristics.

### Dataset Sources

#### 1. Bitcoin Fear & Greed Index

Contains daily market sentiment indicators:

* Date
* Fear & Greed score
* Sentiment classification (Fear, Extreme Fear, Greed, Extreme Greed)

#### 2. Hyperliquid Historical Trading Data

Contains trade-level information:

* Account
* Coin
* Execution Price
* Size (Tokens and USD)
* Side (Buy/Sell)
* Closed PnL
* Fee
* Timestamp
* Position Information

### Methodology

1. Data Cleaning and Preprocessing

   * Standardized timestamps and data types
   * Removed invalid and missing records
   * Merged trading data with sentiment data by date

2. Feature Engineering

   * Trade profitability indicators
   * Trade size metrics
   * Sentiment scores
   * Trader-level performance statistics

3. Exploratory Data Analysis (EDA)

   * Profitability by sentiment
   * Trade volume and activity patterns
   * Buy vs Sell behavior
   * Fee analysis
   * Coin-level performance

4. Trader Segmentation

   * K-Means clustering based on:

     * Total PnL
     * Win Rate
     * Average Trade Size
     * Average Fee
     * Trade Frequency

5. Statistical Validation

   * Mann-Whitney U Test to compare profitability across sentiment regimes

6. Machine Learning

   * Random Forest Classifier
   * Prediction of profitable trades
   * Feature importance analysis

### Key Deliverables

* Comprehensive exploratory analysis
* Statistical comparison of trader performance under different market sentiments
* Trader segmentation and behavioral profiling
* Predictive machine learning model
* Actionable insights and trading recommendations

### Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* SciPy
* Google Colab

### Expected Outcomes

This project aims to uncover whether market sentiment influences trading performance and risk-taking behavior. The findings can help traders and analysts better understand market psychology and develop more informed trading strategies based on prevailing sentiment conditions.
