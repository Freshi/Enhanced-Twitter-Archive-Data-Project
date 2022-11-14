# Data Wrangling - Enhanced Twitter Archive


## Dataset

The dataset is the tweet archive of Twitter user *@dog_rates*, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.The dataset can be found [here]('https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv').

To use the data and conduct the appropriate analysis, we have to enrich the data using the [*Tweet Image Predictions*]('https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv') data that we download using pythons `requests` libary. Using the tweet IDs in the WeRateDogs Twitter archive, we query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called `tweet_json.txt` which we also then use to enrich the archive.

Before analysis, we perform some wrangling that including removing retweets and combining the dog stages into a single variable.




## Summary of Findings

Based on the sums of likes and retweets counts for each breed in our sample, the Labrador and golden
retrievers take the day as the most popular breeds.

From our sample, there seems to be correlation between the *rating* and both the *likes* and *retweet counts*.

We can see that there are a few spikes here and there, but the tweets and retweets are rising albeit slowly over
time.


## More Info
These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because ["they're good dogs Brent."]('https://knowyourmeme.com/memes/theyre-good-dogs-brent')
