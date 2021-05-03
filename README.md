# WeRateDogs_Twitter

WE RATE DOGS: TWITTER RATING ANALYSIS

Introduction:
The following dataset is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators are almost always greater than 10 like 11/10, 12/10, 13/10, etc. The reason why the numerators are greater than denominator is that "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.
WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively to use it as a part of analysis for their student project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

Gathering Data:
Twitter archive file: Provided by udacity. There are 17 columns and 2356 rows in the data set.

Original columns of dataframe are as follows:
tweet_id: the unique identifier for each tweet
in_reply_to_status_id: if the represented Tweet is a reply, this field will contain the integer representation of the original Tweet’s ID
in_reply_to_user_id: if the represented Tweet is a reply, this field will contain the integer representation of the original Tweet’s author ID
timestamp: time when this Tweet was created
source: utility used to post the Tweet, as an HTML-formatted string. e.g. Twitter for Android, Twitter for iPhone, Twitter Web Client
text: actual UTF-8 text of the status update
retweeted_status_id: if the represented Tweet is a retweet, this field will contain the integer representation of the original Tweet’s ID
retweeted_status_user_id: if the represented Tweet is a retweet, this field will contain the integer representation of the original Tweet’s author ID
retweeted_status_timestamp: time of retweet
expanded_urls: tweet URL
rating_numerator: numerator of the rating of a dog. Note: ratings almost always greater than 10
rating_denominator: denominator of the rating of a dog. Note: ratings almost always have a denominator of 10
name: name of the dog
doggo: one of the 4 dog "stage"
floofer: one of the 4 dog "stage"
pupper: one of the 4 dog "stage"
puppo: one of the 4 dog "stage

Twitter download: I had issues with getting access. Hence, used the JSON file provided by Udacity
Columns of the dataframe are as follows:
tweet_id: the unique identifier for each tweet
retweet_count: counts of retweets
favorite_count: counts of likes by people

Libraries:
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
import requests
import tweepy 
import json
import re

Titan version: 3.6.3
