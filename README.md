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

## Conclusion
This project demonstrates how natural language processing techniques can be applied to analyze sentiments in healthcare reviews, providing valuable insights into patient experiences and satisfaction levels. Future work can expand on this foundation by exploring more advanced models or integrating user feedback.

## RESULT 
# Faults from the Dataset Affecting Model Performance:

# Class Imbalance: 
The dataset contains significantly fewer neutral reviews (147 neutral vs. 388 positive and 365 negative). This imbalance causes the models to focus on the more prevalent classes (positive and negative), leading to poor performance in predicting the minority class (neutral). Class imbalance makes it difficult for models to learn an even representation across all categories.

# Limited Dataset Size: 
With only 900 samples, the dataset is relatively small for training machine learning models, especially in a task as nuanced as sentiment analysis. Small datasets can cause models to overfit to the training data and struggle with generalizing to new, unseen examples.

# Simple Sentiment Labeling: 
The sentiment labels are assigned based on numerical ratings (positive, neutral, negative) but may not fully capture the complex emotions and sentiments expressed in the reviews. For instance, a review might have subtle tones of sarcasm, ambiguity, or mixed sentiment, which the label might not fully represent, causing confusion for the models.

# Text Complexity and Ambiguity: 
Sentiment analysis requires understanding context, nuances, and variations in language. The dataset's reviews might contain complex sentences, medical jargon, or mixed sentiment, making it harder for the models to discern clear sentiment using basic feature extraction methods like TF-IDF, which might not capture deeper semantic meaning.

These dataset issues—class imbalance, limited size, simplified labeling, and text complexity—are key factors contributing to the underperformance of the models.