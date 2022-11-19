# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

### Overview
In recent years, Data science has become one of the most popular field. This is all thanks to the rise of technology (especially programming languages, and techniques for collecting, analyzing, and interpreting data). Due to it's popularity, employment of data scientists is projected to grow 36 percent from 2021 to 2031 (much faster than the average for all occupations).
(Source: https://www.bls.gov/ooh/math/data-scientists.htm#:~:text=Employment%20of%20data%20scientists%20is,on%20average%2C%20over%20the%20decade.)

With the increased popularity of Data Science and ease of using Technology to build their own skills sets, there is a greater demand in self learning too. Specifically, Python and Rprogramming are the most popular languages that is in demand. 

### Problem Statement
Although the internet is an efficient and convenient place for self learning, there are also too much content that is available. The resources that have been searched and found, might not be correct/accurate. 
For example, searching for a resolution for Python, might return resolutions for other languages (for example, Rprogramming). 

This project attempts to classify posts/data from Reddit (as a proxy for internet), and identify if it belongs to Python or Rprogramming. 

### Brief summary of your analysis
1. Scrape data from sub-reddit Python and R
2. Clean up data and use the column 'selftext' to classify
3. EDA on scrapped data
4. Modelling 
    - Baseline Accuracy
    - Logistic Regression
    - Random Forests and Extra Trees
    - Support Vector Machines (SVM)

### Conclusions/recommendations
From the models, SVM has best score of 0.9. 
The best parameters are C = 5.0 and Kernel = 'rbf'.
Hence, SVM is the best model to use for classify the posts into identifying whether they are for Python or R.

Moving forward, the below actions are recommended for better classification of the posts:
- Collection of more data
- Using more data columns for modelling (instead of only using 'selftext')
- Run more models to check if there are other models with better performance

