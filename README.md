# WeRateDogs Tweets Analysis

[WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs) 
is a Twitter account ([@dog_rates](https://twitter.com/dog_rates))
that rates people's dogs with 
a humorous comment about the dog. These ratings almost always 
have a denominator of 10. The numerators, though? Almost always 
greater than 10. 11/10, 12/10, 13/10, etc. Why? Because 
["they're good dogs Brent"](https://knowyourmeme.com/memes/theyre-good-dogs-brent).
WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs [downloaded their Twitter archive](https://help.twitter.com/pt/managing-your-account/how-to-download-your-twitter-archive) 
and sent it to 
Udacity via email exclusively for your students to use in this project. 
This archive contains basic tweet data 
(tweet ID, timestamp, text, etc.) for all 5000+ of their tweets 
as they stood on August 1, 2017.

In this project, we will wrangle WeRateDogs Twitter data to create interesting 
and trustworthy analyses and visualizations. The Twitter archive 
is great, but it only contains very basic tweet information. 
Additional gathering, then assessing and cleaning is required 
for "Wow!"-worthy analyses and visualizations.

### Data

The WeRateDogs Twitter archive contains basic tweet data for all 
5000+ of their tweets, but not everything. One column the 
archive does contain though: each tweet's text, which it was used
to extract rating, dog name, and dog "stage" (i.e. doggo, 
floofer, pupper, and puppo) to make this Twitter archive 
"enhanced." Of the 5000+ tweets, 
the data was filtered for tweets with ratings only (there are 2356).

- The extracted data from each tweet text
<img src="https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd4791_screenshot-2017-10-10-18.19.36/screenshot-2017-10-10-18.19.36.png" alt="The extracted data from each tweet text" style="width:800px;"/>


The ratings probably aren't all correct. 
Same goes for the dog names and probably dog stages 
(see below for more information on these) too. 
It will be need to assess and clean these columns if you want to use them 
for analysis and visualization.

- The Dogtionary explains the various stages of dog: doggo, pupper, puppo, and floof(er) (via the #WeRateDogs book on Amazon)
<img src="https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59e04ceb_dogtionary-combined/dogtionary-combined.png" alt="The extracted data from each tweet text" style="width:800px;"/>


### Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two 
of the notable column omissions. Fortunately, this additional data can be gathered by 
anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent 
tweets, at least. The WeRateDogs Twitter archive and specifically 
the tweet IDs within it, it is possible to gather this data for all 5000+. 

### Key Points
Key points to keep in mind when data wrangling for this project:

You only want original ratings (no retweets) that have images. Though there are 5000+ 
tweets in the dataset, not all are dog ratings and some are retweets.
Assessing and cleaning the entire dataset completely would require a lot of time, 
and is not necessary to practice and demonstrate your skills in data wrangling. 
Therefore, the requirements of this project are only to assess and clean at least 8 
quality issues and at least 2 tidiness issues in this dataset.
Cleaning includes merging individual pieces of data according to the rules of tidy data.
The fact that the rating numerators are greater than the denominators does not need to be 
cleaned. This unique rating system is a big part of the popularity of WeRateDogs.
You do not need to gather the tweets beyond August 1st, 2017. You can, but note that you 
won't be able to gather the image predictions for these tweets since you don't have access 
to the algorithm used.

### The tasks in this project are as follows:

1. Data wrangling, which consists of:
	1. Gathering data (downloadable file in the Resources tab in the left most panel of your classroom and linked in step 1 below).
	2. Assessing data
	3. Cleaning data
2. Storing, analyzing, and visualizing your wrangled data
3. Reporting on 1) your data wrangling efforts and 2) your data analyses and visualizations

### Requirements

This project use the follow libraries:
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://www.numpy.org/)
- [Requests](https://2.python-requests.org/en/master/)
- [Tweepy](https://www.tweepy.org/)
- [JSON](https://docs.python.org/3/library/json.html)

To install all the requirements:

```console
$ pip install -r requirements.txt
```

