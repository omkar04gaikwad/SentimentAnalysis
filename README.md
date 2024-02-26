# Logistic Regression: A Sentiment Analysis Case Study

## Introduction

This notebook focuses on performing sentiment analysis using logistic regression on the IMDB movie reviews dataset. The dataset contains 25,000 positive and 25,000 negative reviews, with features represented as a bag of 1-grams with TF-IDF values. Logistic regression is chosen as the classification model due to its ability to handle sparse data and interpretability.

## Task 1: Loading the dataset

The IMDB movie reviews dataset is loaded into a Pandas DataFrame. The dataset consists of positive and negative reviews, and a 50/50 train-test split is employed for evaluation.

## Bag of Words / Bag of N-grams Model

## Task 2: Transforming documents into feature vectors

The CountVectorizer is utilized to construct the vocabulary of the bag-of-words model. The transformed feature vectors are demonstrated on sample sentences.

## Task 3: Word relevancy using term frequency-inverse document frequency

Term frequency-inverse document frequency (TF-IDF) is introduced to assess word relevancy in documents. The TF-IDF values are calculated using scikit-learn's TfidfTransformer.

## Task 4: Data Preparation

Data preparation involves preprocessing the text by removing HTML tags, emoticons, and non-alphanumeric characters. The preprocessor function is applied to the reviews.

## Task 5: Tokenization of documents

Tokenization of documents is performed using NLTK's Porter stemmer. Both a simple tokenizer and a tokenizer with Porter stemming are demonstrated.

## Task 6: Transform Text Data into TF-IDF Vectors

The TfidfVectorizer is used to transform the preprocessed text data into TF-IDF vectors, considering tokenization and Porter stemming.

## Task 7: Document Classification using Logistic Regression

Logistic regression is employed for document classification. The TF-IDF vectors are split into training and testing sets, and logistic regression with cross-validation is utilized for training. The trained model is saved for future use.

## Task 8: Model Evaluation

The saved logistic regression model is loaded and evaluated on the test set, providing the accuracy of the sentiment analysis.

