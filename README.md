## Twitter Sentiment Analysis

  Developing emerging topic detector from Twitter streaming, and performing sentiment analysis on the related tweets to observe the public   opinion on the emerging topic using stateful streaming technique.
  
 ### Emerging topic detection logic 
 
For identifying the emerging topic, one approach can be analysing the contents of the tweets, classifying them into categories and determine the tweets for which the increase in count is maximum. The second approach is identifying the topic based on the hashtag present in the tweet. We used hashtags to identify the emerging topic. 
 
For detecting a rise in the number of tweets over time, we need to maintain the count of the tweets in the previous window duration. This can be achieved using stateful streaming. We used mapWithState and reduceByKeyAndWindow functions for this purpose. 

### Output
**Format -> Current emerging topic, the tweet content for review and its public sentiment**
![alt text](https://github.com/Chitrae92/Twitter-Sentiment-Analysis/blob/master/Output%20Screenshot.PNG)
