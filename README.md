# Sentiment Analysis Cryptocurrency

In this project, I appled natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. I also applied fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

## Sentiment Analysis

Sentiment analysis is a way to quantify the feeling or tone of written text. In sentiment analysis, each case receives a numeric sentiment score (on a negative to positive scale).

I used the newsapi to pull the latest news articles for Bitcoin and Ethereum and created a DataFrame of sentiment scores for each coin. I used descriptive statistics and discovered the following:

* Between Bitcoin and Ethereum, Bitcoin had the highest mean positive score with a score of .096.
* Ethereum had the highest negative with a score of .189.
* Bitcoin had the highest positive score with a score of .169.

## Natural Language Processing

Text may contain stop words like ‘the’, ‘is’, ‘are’. Stop words can be filtered from the text to be processed. The nltk module contains a set list of stop words.
N-Grams are a set of 1 or more consecutive sequence of items that occur next to each other. They can help predict the next words of a text.

I used NTLK and Python to tokenize the text for each coin. Each word is lowercase, all punctuatuion is removed, and all stop words are removed.
I then looked at the ngrams and word frequency for each coin where n = 2 and the top 10 words for each coin are returned.

I then generated word clouds for each coin to summarize the news for each coin.

## Named Entity Recognition

I also built a named entity recognition model for both coins and visualized the tags using SpaCy.
