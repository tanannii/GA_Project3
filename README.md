# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

### Overview
In recent years, Data science has become one of the most popular fields that employees and companies are exploring. Data Science has proven to enable companies to efficiently understand and improve processes. With the increased demand for Data Science employees, there is also a growing group of employees who are upskilling themselves to transit into Data Science roles. With Technology, self learning resources are more accessible and communities for sharing are growing too. Specifically, Reddit is a popular platform for communities to post and share their questions and resolutions. 

### Problem Statement
Although the internet is an efficient and convenient place for self learning, there are also too much content that is available. The resources that have been searched and found, might not be correct/accurate. 
For example, of all the different programming languages that are available, Python is the most popular. However, while searching for a resolution for Python on reddit, it might return resolutions for other languages (for example, SQL). 

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
From the models, Logistic Regression has the highest score of 0.9897. 
Although such high score may signal overfitting, we would go ahead and use Logistic Regression for the ease of explaination and efficiency.

With this model, it can help to better identify if the resolution that was searched was for Python or SQL. This could make learning more efficient and useful. 
Specifically, we have also identified top 'words' that signals stronger. 
The top 5 words that signals that a resolution is 'Python' are:
| Words    | Coefficients |
|----------|--------------|
|   thread |     5.090441 | 
|   pandas |     4.607804 |
| automate |     3.775485 |
|      def |     3.540431 |
|     text |     3.505633 |

For example, as 'thread' appears in a 'selftext' by once, it is about 5.09 times as likely for this resolution to be for 'Python'.

Moving forward, the below actions are recommended for better classification of the posts:
- Collection of more data
- Using more data columns for modelling (instead of only using 'selftext')
- Run more models to check if there are other models with better performance

