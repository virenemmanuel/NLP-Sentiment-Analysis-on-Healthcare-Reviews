# NLP: Sentiment Analysis on Healthcare Reviews

## Overview
This project focuses on analyzing sentiments in healthcare reviews. The objective is to develop a model that classifies sentiments expressed in the reviews into three categories: positive, neutral, and negative. 

## Problem Statement
Healthcare reviews often reflect patients' experiences, emotions, and opinions about the services they receive. Analyzing these sentiments can provide valuable insights into patient satisfaction and areas needing improvement.

## Objectives
- Develop a sentiment analysis model to classify healthcare reviews.
- Visualize sentiments using word clouds for better insights.

## Tasks
1. **Data Preprocessing**
    - Load the dataset and handle missing values.
    - Clean the review text by removing HTML tags, punctuation, and stop words, and applying lemmatization.

2. **Sentiment Analysis Model**
    - Classify sentiments based on ratings:
        - Positive sentiment (`1`) for ratings above 3.
        - Neutral sentiment (`0`) for ratings equal to 3.
        - Negative sentiment (`-1`) for ratings below 3.
    - Handle class imbalance using SMOTE to ensure a balanced dataset for training.
    - Use TF-IDF for text vectorization.
    - Train a logistic regression model to classify sentiments.

3. **Model Evaluation**
    - Evaluate the model performance using metrics such as precision, recall, and F1-score.
    - Display the confusion matrix to visualize model performance.

4. **Insights & Visualization**
    - Visualize sentiment distribution using bar charts.
    - Generate word clouds for positive, negative, and neutral sentiments to highlight common words used in reviews.

## Requirements
- Python 3.6+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `nltk`, `wordcloud`, `imbalanced-learn`



