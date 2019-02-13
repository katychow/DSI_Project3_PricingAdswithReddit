## Project 3 README

The **_objective_** of Project 3 was to be able to use classification methods and run an experiment on whether or not one could predict the correct subreddit

## Executive Summary

Reddit is starting to sell advertising space in subreddits.  They want a tiered structure to pricing based on post popularity.  (eg. if a post is more popular, it will cost more for ad space within a subreddit) It seems as though while we are very good at predicting the correct subreddit, we are not very good at predicting the up votes.  Perhaps a better marketing strategy would be to predict which subreddits are the most popular on the hot page and price advertisements based on the subreddit.

## Data Information

Data scraped from subreddits are the [psychology](https://www.reddit.com/r/psychology) and [mental health](https://www.reddit.com/r/mentalhealth) subreddit.  

#### Data Dictionary of Data Pulled
|Column Name | Data Type | Brief Description |
|---|---|---|
|subreddit|str|subreddit data pulled from|
|title|str|title of pose in subreddit|
|num_comments|int|number of comments|
|ups|int|up votes of post|
|downs|int|down votes of posts|
|likes|int|likes of posts|
|view_count|int|counts of times post viewed|
|url|str|url for subreddit post|
|time_of_pull|timestamp|time when post was scraped|


## How to Navigate Folders and Files

1. **_Code_** Folder, 4 Files, Organized with _NB suffix
  * NB1 contains code to scrape subreddit data
  * NB2 contains code to run models to classify subreddit data and determine if the title of a subreddit is either mental health or psychology, some visualizations at the end from using sentiment analysis
  * NB3 contains code to run adhoc visualizations including word cloud code and also lots of histograms
  * NB4 contains code to run models on prediction of 'ups' given a specific subreddit
<br><br>
2. **_Data_** Folder, 6 Files
  * Subreddit webscrape data denoted by Reddit_**Subreddit Name Here**_datefilewritten.csv
  * 4 subreddit webscraped data files, used Reddit_MH, most current version of Reddit_Psych for project
  * other files include, "train" dataset intended for visualizations and coefficient values of classification model in CSV format
<br><br>
3.  **_Images_** Folder, 22 Files
  * Wordcloud images denoted by suffix of _wordcloud
  * histograms of Top20 words for each subreddit and both subreddits combined denoted by prefix of Top20
  * scatterplots of sentiment analysis comparing pos,neg,neu scores to the compound scores denoted by prefix of RedditComparisonsSentiments
  * a few model flow charts denoted with psycho-or-mentalhealth prefix
  * other images contain misnamed versions of above, the background image for wordclouds, and histogram comparing words across both subreddits.
<br><br>
4. **_Misc_** Folder, 3 Files
  * 2 files regarding project instructions
  * 1 file as a template for KatyChow_README.md file on first page
