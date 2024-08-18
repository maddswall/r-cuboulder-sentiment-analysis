# Project Overview
This project leverages topic modeling and sentiment analysis on the r/CUBoulder subreddit to understand public perception of the University of Colorado at Boulder.

# Data Collection
Reddit API Scraper: We obtained, cleaned, and organized our own data from Reddit using PRAW (Python Reddit API Wrapper).

# Data Preprocessing
Stop Words Removal: We utilized the Natural Language Toolkit (NLTK) library to remove common stop words (e.g., "and," "the") from the comments.

# Lemmatization
Using NLTK, we created a custom function to lemmatize words based on their part of speech. This involved tokenizing comments, applying part-of-speech tagging, and reducing words to their base form using the WordNetLemmatizer module. Lemmatization is crucial for grouping variations of the same word together, enhancing the accuracy of our analysis.

# Topic Modeling
BERTopic: We used BERTopic for topic modeling. BERTopic leverages BERT embeddings and c-TF-IDF to create dense clusters, allowing for interpretable topics while retaining important words in the topic descriptions.

# Sentiment Analysis
Unsupervised Sentiment Analysis: Given the absence of labeled data, we employed VADER (Valence Aware Dictionary and sEntiment Reasoner), an unsupervised sentiment analysis tool from NLTK. VADER enables accurate sentiment measurement in unlabeled data, making it an ideal choice for our project.
