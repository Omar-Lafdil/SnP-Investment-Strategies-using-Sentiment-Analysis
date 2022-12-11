# SnP-Investment-Strategies-using-Sentiment-Analysis

The Client's Requirements :

1. Jupiter Notebook
Obtain financial news (ESG and market) from 01.01.2014 from Reuters (30 articles per day each – title & content). If Reuters data is not enough, then get it from other sites such as Bloomberg, Wall Street Journal, Yahoo, etc. The data can be obtained through Beautifulsoup.

2. Jupiter Notebook 
FinBERT preparation (https://medium.com/prosus-ai-tech-blog/finbert-financial-sentiment-analysis-with-bert-b277a3607101) as in this link with TRC2, Hugging Face's and Financial Phrase Bank. If FinBERT can be obtained directly via a Python function, then do so if the pre-training was also exactly as described above. Describe the parameters of the model.
In a further step, the sentiment scores are to be calculated from the news obtained per day. 
https://medium.com/@ravirajshinde2000/financial-news-sentiment-analysis-using-finbert-25afcc95e65f

Sentiment score calculation: 
-	Sentiment for a sentence = probability of a positive sentence – probability of a negative sentence 
-	The sentiment score for the whole text = average of the sentiments form the sentences

 The news of today = Sentimentscore of tomorrow
 The news from Friday, Saturday and Sunday is the Sentiment of Monday

-> If more than 50% of the news was positive, then the feature should be 1.
-> if less than 50% = -1 and if exactly 50% = 0
If FinBERT cannot be obtained directly, please also send the three databases mentioned. 
Visualisation of how much is positive, negative, and neutral

3. Jupiter Notebook
Obtain data from S&P500 (01.01.2014 - 28.11.22) and invest or close position in S&P based on the newly generated feature. If the feature is 0, then no trading is done on that day. 

On the first day, a positive sentiment is assumed and therefore also invested. (Since we do not have a sentiment score from yesterday = endless loop).

Visualisation of the timeseries before and after. In addition, show in the chart how many tradings have been made.


-> The codes should be as simple as possible with a comment on what exactly is done in the code line.

