# Ethereum Sentiment Analysis for Price Movement Prediction

### Objective statement:

Celebrities usually have a huge influence on the society, and financial industry is no exception . For example, Elon Musk, the founder and CEO of Telsa; he is a significant social media influence, In the last week of march it happened, Just after midnight on Monday morning, in a Twitter thread about inflation, the Tesla CEO tweeted that he would not be selling his crypto holdings, which include unknown quantities of Dogecoin, Bitcoin, and Ether. Minutes later, Dogecoin reached its highest price in the last five days. It's certainly not the first time Musk has tweeted about DOGE. In January and February, he tweeted about the cryptocurrency repeatedly, leading to price surges each time. He began vaguely, and gradually became more.

### There are four clear benefits of using machine learning and artificial intelligence to set the pricing strategy. ​

1. ML can cope with price volatility:

    Price volatility denotes the price fluctuations of a product. To measure price volatility, you need to take a day-to-day percentage difference in a product or service’s price. In the context of the stock market, where prices can change in milliseconds, this type of capability is invaluable. The system can analyze and respond to a myriad of factors in fractions of a second, which is something a human never could.

2. ML models can analyze multiple data sources at once
    
    Price prediction is hard because it requires many data sources: from internal market reports to competitors’ webpages to CRM files. And it’s a challenge for humans to process this volume of information, whereas, for AI, more data is nearly always better.

3. ML improves the accuracy of price movement predictions

    The accuracy of traditional pricing methods leaves much to be desired. In truth, most conventional methods value intuition and subjective opinion over hard data. And that’s why decisions based on such processes often lead businesses down a rabbit hole.

4. ML can help you improve your profit margin

    When you use machine learning, you also get an excellent grasp of how industry prices evolve over the course of a year. And this leads to a final, more subtle benefit.

### Goal:  To find the Leading Indicator of Ethereum

A leading indicator looks forward to future outcomes and events, hence, if a leading indicator is found, it is a good prediction of what will happen to the price movement of an asset. In this case, analyzing millions of tweets related to Ethereum to predict the price of the Ethereum, and to make buy and sell decision based on these predictions

### Approach: 

##### The Machine Learning 

Price Analysis

Sentiment Analysis

Tweet sentiments indicator calculation 

##### Investment Strategy

Price Momentum strategy

Contrarian strategy

### Factors that could  be used to fetch meaningful tweets from Twitter:

1. Popular personalities like Joseph Lubin, Vitalik Buterin, Ashton Kutcher etc. should  be good indicator for Ethereum prices.

2. Corporations like Galaxy Digital Holdings are good indicator, as they are biggest investors in Ethereum.

3. We are trying to use retweets count for every tweet, as big weightage behind positive or negative sentiments. Generally, people tend to retweet positive news.

4. Language – English is our language of interest for our ML model, so we tried fetching English tweets only.

5. Bias – We need to filter out tweets which are not conveying any sentiments, just sharing some general information. What if someone trying to spreading positive fake news, even if Ethereum going down.

6. Tweet Volume – This is a good indicator about people’s interest in particular topic or hashtag.

### Model:

1. Data Collection: Fetch Tweet: Historical data, Twitter API or Tweepy Library​

2. Data Preprocessing: Removal using NLTK

3. Sentiment Analysis: Flair on past 7 days

4. Application of Sentiment: Emphasize by assigning binary values (+1/-1)

### Solution: 

![image](https://user-images.githubusercontent.com/94947162/229944720-8e292409-200a-414e-8093-86b50ddab4c7.png)

The first graph shows the Ethereum closing price over the 7-day period; April 9-15th. Graph2 shows the daily overall sentiment point as calculated in our model. The third graph indicates the total positive, total negative, and proportion of positives compared to negatives each day which is indicated by the blue line. After we have 7 days worth of sentiment, we apply 2 investment strategies: contrarian, and price momentum. Applying price momentum strategy on the price analysis done on the first step, price will likely increase, as it follows fall-rise-fall-rise pattern, hence we buy. Keeping in mind it is difficult to predict due to heavy fluctuation and lack of sufficient data. Notice there has been consistent overall positive tweets but the total number of positive proportion is decreasing. Applying contrarian strategy, we buy as the sentiment towards Etheruem is going down.  On April 16th, which is the day after our 7 day prediction, the price actually did go up from $3040 to $3060. Voila! However, its fluctuation make the model very difficult to predict after that. The last graph shows Ethereum price from April 15-21st. A increase on the next day, but shortly a dip then goes back up but hit very low after 4 days.

### Future Scope:

There should be asset classes with a positive or negative correlations with Ethereum.  To make the model more accurate and to use algorithm to search for asset classes with strong correlations. For instance, Graphic Processor company such as AMD produces processors that are crucial for the mining of crypto, hence there should be correlations between the two Likewise, logically crypto currencies will play a critical role as the trading medium in the Metaverse, hence, Metaverse developers such as Meta's (aka Facebook's) development and succuss in developing the Metaverse would impact the adaption and therefore the price of crypto. 
