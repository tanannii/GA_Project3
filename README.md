# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

### Overview
In recent years, Data science has become one of the most popular field. This is all thanks to the rise of technology, making accessibility to resources a lot easier (especially programming languages, and techniques for collecting, analyzing, and interpreting data). Due to it's popularity, employment of data scientists is projected to grow 36 percent from 2021 to 2031 (much faster than the average for all occupations).

(Source: https://www.bls.gov/ooh/math/data-scientists.htm#:~:text=Employment%20of%20data%20scientists%20is,on%20average%2C%20over%20the%20decade.)

With the increased popularity of Data Science and ease of using Technology to build their own skills sets, there is a greater demand in self learning too. Specifically, Python and Rprogramming are the most popular languages that is in demand. 

### Problem Statement
Although the internet is an efficient and convenient place for self learning, there are also too much content that is available. The resources that have been searched and found, might not be correct/accurate. 
For example, searching for a resolution for Python, might return resolutions for other languages (for example, Rprogramming). 

This project attempts to classify posts/data from Reddit (as a proxy for internet), and identify if it belongs to Python or SQL. 

### Brief summary of your analysis
1. Scrape data from sub-reddit Python and R
    - https://www.reddit.com/r/SQL/
    - https://www.reddit.com/r/Python/
3. Clean up data and use the column 'selftext' to classify
4. EDA on scrapped data
5. Modelling 
    - Baseline Accuracy
    - Logistic Regression
    - Random Forests and Extra Trees
    - Support Vector Machines (SVM)

### Conclusions/recommendations
From the models, Logistic Regression has the highest score of 0.9972. 
Although such high score may signal overfitting, we would go ahead and use Logistic Regression for the ease of explaination and efficiency.

With this model, it can help to better identify if the resolution that was searched was for Python or SQL. This could make learning more efficient and useful. 
Specifically, we have also identified top 'words' that signals stronger. 
The top 5 words that signals that a resolution is 'Python' are:
| Words  | Coefficients |
|--------|--------------|
|  https |     7.919949 |   
|  x200b |     5.233946 |   
| github |     4.656340 |  
|    api |     3.966020 |   
| thread |     3.618439 |   
For example, as 'https' appears in a 'selftext' by one unit, it is about 7.92 times as likely for this resolution to be for 'Python'.

Moving forward, the below actions are recommended for better classification of the posts:
- Collection of more data
- Using more data columns for modelling (instead of only using 'selftext')
- Run more models to check if there are other models with better performance

