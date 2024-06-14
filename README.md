# Novo Trustpilot Reviews Sentiment Analysis

## Overview
This project aims to analyze and classify user reviews from Novo Trustpilot ratings. The primary objective is to identify the intent behind each review, such as 'Lost Password', 'Account Setup', 'Positive Feedback', etc., using natural language processing (NLP) techniques and machine learning models.

## Approach

### 1. Taxonomy Development
- **Data Preprocessing**: Cleaning the text data by removing non-alphabetical characters and converting text to lowercase.
- **Tokenization and Lemmatization**: Breaking down the text into tokens and normalizing words to their base form.

### 2. Model Training
- **Word Embeddings**: Creating word embeddings using Word2Vec to convert text into numerical vectors.
- **Intent Classification**: Using LSTM (Long Short-Term Memory) neural networks to classify the intent of each review.

### 3. Model Evaluation
- **Performance Metrics**: Evaluating the model using accuracy and loss metrics.
- **Validation**: Splitting the dataset into training and testing sets to validate the model's performance.

## Tradeoffs and Challenges
- **Data Imbalance**: Some intent categories had significantly more examples than others. Addressing this required careful data sampling and weighting during model training.
- **Text Ambiguity**: User reviews often contain ambiguous language, making intent classification challenging. The use of advanced NLP techniques and fine-tuning of models helped mitigate this issue.

## Model Performance
- **Accuracy**: The final model achieved an accuracy of approximately 65% on the test dataset.
- **Loss**: The model's loss on the test dataset was approximately 1.29.

## Prompt Engineering Examples
- **Positive Feedback**: "Great service, highly recommend!"
- **Account Setup**: "It was easy to set up a new account."
- **Service Issues**: "I had problems with the customer service."

## Future Plans
- **Continuous Improvement**: Regularly updating the model with new reviews and intents.
- **Enhanced Features**: Incorporating additional features such as review metadata and user profiles to improve intent classification.
