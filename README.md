
# 📊 Market Sentiment vs Trading Performance Analysis

An exploratory data analysis project to understand how market sentiment impacts trading profitability, risk, and trading behavior.



## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Tools and Technologies](#tools-and-technologies)
- [Methods](#methods)
- [Findings & Insights](#findings-&-insights)
- [Output](#output)
- [How to Run This Project](#how-to-run-this-project)
- [Results & Conclusion](#results--conclusion)
- [Future Work](#future-work)
- [Author & Contact](#author-&-contact)



## Overview

Financial markets are heavily influenced by emotions such as fear and greed. This project analyzes historical crypto trading data combined with the Fear & Greed Index to study how different sentiment regimes affect trader profitability, volatility, and capital deployment. The goal is to uncover patterns that can help traders and analysts make more informed, sentiment-aware decisions.




## Problem Statement

Does market sentiment meaningfully influence trading outcomes?
Specifically:

- How does profitability vary across different sentiment regimes?
- Are emotional market phases riskier than neutral phases?
- Does higher trading activity always lead to better performance?


## Dataset

This project uses two datasets:

**1. Historical Trader Data**

Trade-level data including position size, profit/loss, timestamps, and token quantities.

**2. Fear & Greed Index**

Daily market sentiment classified into categories such as Extreme Fear, Fear, Neutral, Greed, and Extreme Greed.

Both datasets were merged using date alignment to enable sentiment-based analysis.
## Tools and Technologies

- **Python**

- **Pandas** – data cleaning, transformation, aggregation

- **Matplotlib & Seaborn** – data visualization

- **Google Colab** – development environment

- **GitHub** – version control and project sharing

## Methods

- Cleaned and standardized date formats across datasets

- Merged trading data with daily sentiment classifications

- Analyzed profitability using mean and volatility (standard deviation) of Closed PnL

- Evaluated trading behavior using USD volume and token volume

- Visualized insights using bar charts to capture both trends and distributions

# **📊 Key Findings & Insights**


![Sentiment Analysis Visualisation](https://github.com/rahulssg/market-sentiment-trading-analysis/blob/master/outputs/Sentiment%20Analysis%20Results.png?raw=true)


## **Finding 1: Profitability and volatility vary significantly across market sentiments**

From the profitability and risk analysis, Extreme Greed shows the highest average Closed PnL (around $67.9), followed by Fear (around $54.3). However, the highest risk, measured through standard deviation, appears during Extreme Fear (about 1136), closely followed by Greed (around 1116). In contrast, the Neutral sentiment phase has the lowest volatility at around 517.

### **Insight:**
This indicates that although the best average profits tend to occur during very optimistic market conditions, these phases are also highly unstable. Emotional extremes—both fear and greed, lead to large fluctuations in outcomes. Neutral market conditions are much balanced but offer fewer opportunities for high returns.

## **Finding 2: High capital deployment does not translate directly into higher profits**

The trading volume analysis shows that Fear has the highest total trading volume in USD, at approximately $483 million. However, this sentiment phase does not produce the highest average profitability, which instead occurs during Extreme Greed.

### **Insight:**
This suggests that during fearful markets, traders deploy more capital defensively or reactively, rather than in a way that maximizes returns. In other words, trading more or committing more money does not automatically lead to better profitability.

## **Finding 3: USD volume and token volume reflect different trading behaviors**

While Fear is associated with high USD trading volume, it shows relatively lower token activity. On the other hand, Extreme Greed has a much higher number of tokens traded (around 353 million) despite a lower total USD volume (around 124 million).

### **Insight:**
This pattern suggests that during fearful periods, traders may be cautious and focus on fewer or higher-priced assets. In contrast, during extreme greed, traders aggressively accumulate larger quantities of tokens, possibly driven by strong bullish sentiment or fear of missing out (FOMO), rather than price sensitivity.

## **Finding 4: Neutral sentiment offers stability but limited upside**

The Neutral sentiment phase shows moderate trading volumes and the lowest volatility in Closed PnL, along with relatively average profitability levels.

### **Insight:**
This indicates that neutral market conditions are more predictable and less risky, making them suitable for capital preservation. However, they do not offer strong profit-generating opportunities, as emotional and momentum-driven trades are limited.

# **Final Recommendations**

- Use market sentiment as a regime filter to adjust position sizing and overall trading aggressiveness.

- Focus on Extreme Greed phases for higher return opportunities, but apply strict risk management controls.

- Reduce exposure or trade selectively during Extreme Fear due to high volatility and unpredictable outcomes.

- Prioritize capital preservation strategies during Neutral sentiment, as stability is higher but profit potential is limited.

## Output

The project includes:

- Bar charts comparing average profitability and volatility across sentiments

- Volume analysis visualizations (USD vs token activity)

- All generated visuals are stored in the Output/ folder.

## How to Run This Project

- Clone or download this repository

- Ensure required libraries are installed (pandas, matplotlib, seaborn)

- Open analysis.ipynb in Jupyter Notebook or Google Colab (**Colab Link:** https://colab.research.google.com/drive/1Q97fUFPi58ICNzLdpiQYTK-t1uVNLy2j?usp=sharing)

- Ensure CSV files are present in the csv_files/ directory

- Run the notebook top-to-bottom to reproduce the analysis

## Results & Conclusion

The analysis confirms that market sentiment significantly influences trading outcomes. Emotional extremes increase both opportunity and risk, while neutral markets provide stability with limited upside. These findings highlight the importance of adapting trading strategies and risk management based on prevailing market sentiment rather than relying solely on trade volume or activity.

## Future Work

- Incorporate time-series analysis to study sentiment shifts over time

- Analyze individual trader behavior instead of aggregate performance

- Extend the study to additional market indicators (volatility index, funding rates)

- Build an interactive dashboard for real-time sentiment-based insights

# Author & Contact
## Rahul Singh
🔗 [LinkedIn](https://www.linkedin.com/in/rahul-singh-825450215)
