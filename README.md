# Project 3: Web APIs & NLP

## Problem Statement

A popular online superhero merchanise company called Superherostuff (https://www.superherostuff.com) wants to catergorize customer posts on its online review page as either Marvel or DCComics fans. A data scientist has been hired to successfully develop a classification model based on posts from two popular subreddits, r/Marvel and r/DCComics and validate its accuracy.This model would then be used by the company to categorize customer reviews. 

## Executive Summary

The following questions were answered using the finalized model:
- What words were most frequent from both subreddits?
- Were there any words that were common between both subreddits?
- What was the baseline model accuracy?
- What was the best model accuracy?
- How can the model be further improved?

## Data Dictionary 

The following data was scraped from Reddit
Source:https://praw.readthedocs.io/en/latest/code_overview/models/subreddit.html

|Feature|Type|Description|
|---|---|---|
|**Id**|*string*|ID of the subreddit post|
|**subreddit**|*string*|Name of the subreddit|
|**title**|*string*|The title of the submission|
|**selftext**|*string*|The markdown formatted content for a text submission|

## Conclusions and Recommendations

The best classifier model was a Multinomial Naive Bayes Classifier using Count Vectorizer with a good accuracy score of 94.3%.

The best model score was a huge improvement than guessing wherever a post belonged to the Marvel subreddit or not 50.2% of the time.

The model can be further improved by looking into the posts that were misclassified.

Hyperparameters can be further explored and finetuned for various models that were analyzed.

The total dataset consisted of only 3000 subreddit posts. Maybe more subreddit posts can be webscraped from the reddit platforms to construct a more generalized model and avoid overfitting.

For this project, only the subreddit posts were considered. As an extension to improve the model, the comments and self text columns can be considered as well.

Subreddit posts from a non biased subreddit like r/Comics can be classified to further validate the accuracy of the model.
