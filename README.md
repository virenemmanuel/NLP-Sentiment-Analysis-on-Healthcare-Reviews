# NLP: Sentiment Analysis on Healthcare Reviews

# DOMAIN : Healthcare

## Overview
This project focuses on analyzing sentiments in healthcare reviews. The objective is to develop a model that classifies sentiments expressed in the reviews into three categories: positive, neutral, and negative. 

## Problem Statement
Healthcare reviews often reflect patients' experiences, emotions, and opinions about the services they receive. Analyzing these sentiments can provide valuable insights into patient satisfaction and areas needing improvement.

## Objectives
- Develop a sentiment analysis model to classify healthcare reviews.
- Visualize sentiments using word clouds for better insights.

## Tasks
 ## 1.Data Preprocessing
    Lowercasing: Convert text to lowercase.
    Text Cleaning: Remove unwanted characters and symbols.
    Tokenization: Split text into words.
    Stopword Removal: Remove common, unimportant words.
    Lemmatization: Reduce words to their base form.
    Stemming: Remove suffixes to get the root form of words.
    POS Tagging: Identify grammatical categories (e.g., nouns, verbs).
    Polarity: Assign sentiment labels (positive, negative, neutral).
    Text Vectorization: Convert text to numerical vectors (e.g., TF-IDF).
    Imbalance Handling: Use SMOTE to balance class distribution. 

 ## 2.Sentiment Analysis Model
   The Sentiment Analysis Model is central to this project, where machine learning algorithms are trained to classify reviews into three sentiment categories: positive, negative, or neutral. The following classification models are explored:


   #Random Forest: 

      An ensemble model that combines multiple decision trees to 
      improve classification accuracy by reducing overfitting.

   #Naive Bayes: 
   
      A probabilistic model based on Bayes' theorem, often used for 
      text classification by calculating the likelihood of a review 
      belonging to each sentiment class.

   Support Vector Machine (SVM): 

      A classifier that separates classes using a hyperplane, 
      handling both linear and non-linear sentiment classification tasks.

   Logistic Regression: 

      A linear classifier that models the probability of a review 
      belonging to a specific sentiment class (positive, negative, or neutral).
    
   


 ## 3.Model Evaluation
  
    Model evaluation is crucial for assessing the performance of sentiment analysis models. 
    Key metrics include accuracy, precision, recall, and F1-score. 
    Cross-validation and hyperparameter tuning are employed to optimize model performance.

    - Evaluate the model performance using metrics such as precision, recall, and F1-score.
    - Display the confusion matrix to visualize model performance.

Training Data

    The models have achieved perfect accuracy on the training set, 
    as evidenced by the training accuracy of 1.00.
    The classification report and confusion matrix suggest that the model 
    is making correct predictions for each class, with precision, recall, 
    and F1-score all equal to 1.00

Testing Data

   The model achieved perfect accuracy on the test set, 
   which aligns with the results on the training set.
   The classification report and confusion matrix suggest that 
   the model is making correct predictions for each class, with precision, recall, 
   and F1-score all equal to 1.00.

Cross-Validation of Models

   All individual cross-validation accuracy scores on the training and testing data are 1.0 (100%). 
   This suggests that, in each fold, the model achieved perfect accuracy 
   on the training and testing data.
   The mean accuracy on the training and testing data is also 1.0, 
   indicating that the model consistently performed well across different subsets 
   of the training and testing data during cross-validation
   In summary, High accuracy on the testing set is indicative of a 
   well-performing model. The model appears to generalize well to different subsets of 
   both the training and testing data, as indicated by the consistent perfect accuracy 
   scores in cross-validation as well. It is essential to approach model evaluation 
   with a critical eye and consider the broader context of the dataset and problem


## 4. Insights and Visualization
In this phase, the project aims to derive actionable insights from the sentiment analysis results. 
Visualizations, such as word clouds and sentiment distribution plots, 
help in presenting findings in an interpretable manner.

Count of sentiments: Sentiment Count Positive reviews 515 Negative 387 Neutral 98

Top 10 Recurring Words:

experience
service
provider
healthcare
bad
im
satisfied
received
highly
recommended
Most frequently used words: Positive Reviews:

service 208
highly 117
satisfied 117
recommended 117
received 117
Customers are highly satisfied and recommend the service.
Negative Reviews :

experience 281
provider 187
bad 184
service 106
disappointing 106
Customers had a bad, disappointing experience and service.
Neutral Reviews:

experience 281
provider 187
bad 184
service 106
disappointing 106
Customers had a bad, disappointing experience and service.
Recommendations


1. Address Negative Reviews:

Common Issues: Analyzing negative reviews identified common issues or concerns raised by patients are bad service is provided and they are disappointed.
Root Cause Analysis: Conduct a root cause analysis to understand the underlying problems leading to negative feedback.
Implement Solutions: Develop and implement action plans to address the identified issues.


2. Promote Positive Reviews:
Encourage Feedback: Actively encourage patients to leave reviews, especially those who have had positive experiences.
Highlight Success Stories: Share positive patient stories and testimonials on the hospital's website or social media to build trust.

3. Improve Communication:
Patient Communication: Enhance communication between medical staff and patients. Ensure that information about procedures, treatments, and recovery plans is conveyed clearly.
Feedback Mechanism: Establish a feedback mechanism for patients to share concerns and suggestions during their stay.

4. Staff Training:
Customer Service Training: Provide ongoing training for hospital staff in customer service and patient communication.
Empathy and Compassion: Emphasize the importance of empathy and compassion in patient interactions.

5. Quality of Care:
Clinical Excellence: Prioritize and continually improve the quality of medical care and services provided.
Patient Outcome Monitoring: Regularly monitor patient outcomes and take measures to enhance medical performance.

6. Patient-Centered Approach:
Patient Satisfaction Surveys: Conduct regular patient satisfaction surveys to gather feedback on various aspects of their experience.
Patient-Centered Policies: Implement policies that prioritize the comfort and well-being of patients.

7. Online Presence
Responsive Online Presence: Maintain an active and responsive online presence. Address reviews and concerns promptly.
Educational Content: Share educational content and resources on the hospital's website to keep patients informed.

8. Employee Well-being:
Staff Support Programs: Implement programs to support the well-being and mental health of hospital staff.
Recognition and Incentives: Recognize and reward staff for excellent patient care and positive contributions.

9. Continuous Improvement:
Performance Metrics: Establish key performance indicators (KPIs) to measure hospital performance and continuously improve based on data.
Regular Audits: Conduct regular internal audits to assess adherence to quality standards and patient satisfaction.