# Twitter-User-WeRateDog-Data-Analysis

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog, and these ratings almost always have a denominator of 10. 
This report documents the steps taken to gather, clean and store the data.

The dataset used in this project were gotten from three sources:

- The first dataset is from the WeRateDogs downloaded Twitter archive. 
This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ oftheir tweets as they stood on August 1, 2017.
The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. 
One column the archive does contain though: each tweet's text, 
which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, 
I have filtered for tweets with ratings only (there are 2356).

- Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. 
Fortunately, this additional data can be gathered by anyone from Twitter's API. 
I used the tweet IDs from WeRateDogs Twitter archive to gather the the missing data for all 5000+ tweets. 
These valuable data were gathered by querying Twitter's API.

- The third data used was the image files of all the dog tweets

After combining the datasets, it was trimmed down to 1906 rows and twelve columns and the
analysis was carried out to answer the following questions;
 
 	- What is the top source, users tweeted from?
 	- The top 10 most popular dog breed in the tweets
 	- Top rated dog based on retweets
 	- Top rated dog based on favorite count
 	- The winner of the contest, which is top rated based on dog rating and retweet count and favorite count
