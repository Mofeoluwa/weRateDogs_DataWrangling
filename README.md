# weRateDogs_DataWrangling

### Datasets Description 

There are three sources of data in this project.
1.	Basic archived data from weRateDogs, aka archive_df.
2.	Dog breed prediction was provided by a volunteer who used a neural network classification process on images attached to tweets, aka image_predictions.
3.	Live data tweets are downloaded using the Twitter API, aka tweet_df.


### Issues in each dataset
1.	The tweet_df had one quality issue; the tweet_id should not be an int datatype. However, the data frame was well structured since only the tweet_id, retweet_count, and favorite_count was extracted.


2.	The image_predictions data frame had one quality issue; the tweet_id should not be an int datatype. The data frame was not well structured as there are multiple rows of predictions, prediction confidence, and the likelihood of prediction being True and False. Each of these values needed to be merged to make better sense of the data.



3.	The archive_df data frame had several quality and tidiness issues.
The tweet_id should not be an int datatype.
The entries for retweeted tweets should be dropped as this analysis focuses on original tweets.
The replies to tweets should also be dropped.
The timestamp column should be a Datetime datatype, not an object.
The rating_denominator must be set to 10 because, as stated earlier, the denominator is usually 10.
The data frame was poorly structured, with multiple rows of dog stages. The Doggo, Floofer, Pupper, and Puppo columns need to be merged to make better sense of the data.

### Insight and Visualization
During the visualization of the weRateDog Twitter account tweets, I focused on getting the following insights:
1.	The distribution of the source of tweets
2.	The distribution of the stages of dogs in the tweets
3.	The most common names by frequency 
4.	The most common breeds by frequency
5.	The most common names by number of retweets and likes
6.	The most common breeds by number of retweets and likes


