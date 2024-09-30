# Sentiment-Analysis_NLP

## Introduction
- In the rapidly evolving tech market, consumer feedback is crucial for shaping product development and marketing strategies. Analyzing customer sentiments expressed in online reviews helps businesses align their offerings with consumer expectations.
- With the rise of online shopping, analyzing customer sentiments has become essential to understand consumer demands and improve business decisions.
- This project focuses on analyzing customer sentiments towards iPhone products using Natural Language Processing (NLP) techniques, particularly by scraping reviews from Amazon and extracting valuable insights from them.

## Aim of the Study
To analyze customer sentiment towards iPhone products using NLP techniques on Amazon reviews.

## Objectives of the Study
- **Primary Goal**: To analyze customer sentiment towards iPhone products using NLP techniques on Amazon reviews.
  
### Specific Objectives:
1. **Collect and Pre-process Data**: Gather iPhone product reviews from Amazon using web scraping techniques and preprocess the data.
2. **Perform Sentiment Analysis**: Apply various sentiment analysis models to determine the polarity of reviews (positive or negative).
3. **Model Comparison**: Compare sentiment analysis models to find the best fit for predicting sentiments and assess overall customer satisfaction.

## Dataset Overview
- **Source of Data**: Reviews of iPhone products sourced from Amazon through web scraping.
  
## Graphical Visualizations / Exploratory Data Analysis (EDA)
1. **Count Plot**: 
   - Displays the distribution of positive and negative sentiments in the dataset.
   - Positive Reviews: 711
   - Negative Reviews: 283
2. **Word Cloud Analysis**: 
   - Identifies key themes and frequently occurring words in review texts.

## Preprocessing Steps
1. **Remove Stopwords**: Eliminate common, non-informative words to focus on meaningful content.
2. **Drop Duplicates**: Ensure the dataset is unique and free from redundancy.
3. **Preprocess Text**:
   - Tokenization
   - Convert to lowercase for uniformity
   - Remove stopwords again after tokenization
4. **Convert Emojis to Text**: Translate emojis into textual descriptions to capture sentiment.
5. **Handle Negation**: Account for phrases like “not good” that change sentiment polarity.
6. **TF-IDF Vectorizer**: Transform text into numerical features for use in machine learning models.

## NLP Models Used
1. **Multilingual-BERT**: 
   - Classifies sentiment with results >3 as positive, and ≤3 as negative.
   - **Why Use BERT?**: BERT captures deep contextual information from the text and is language-flexible, handling multiple languages and nuances in sentiment.
   
2. **Alternative Models**:
   - **VADER**: Effective for social media text and informal language.
   - **TextBlob**: Simple and effective for basic sentiment analysis.
   - **FastText**: Efficient for large datasets but lacks deep contextual understanding.
   - **GPT-based Models**: Advanced, context-aware models.
   - **SentiWordNet**: Assigns sentiment scores to words based on WordNet.
   - **Polarity Score**: Quantifies the sentiment on a scale from negative to positive.

## Model Selection and Training
1. **Models Explored**:
   - **SVM (Support Vector Machine)**: Finds the optimal boundary between sentiment classes.
   - **Naive Bayes**: Probabilistic classifier that assumes independence between features.
   - **Random Forest**: Ensemble method that aggregates decision tree outputs.

2. **Training Details**:
   - **Train-Test Split**: An 80-20 split was used to train the models.
   - **Class Imbalance Handling**: SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset.
   
## Results and Conclusion
- **Best-Performing Model**: Random Forest, which showed the highest accuracy and balanced metrics across sentiment categories.
- **Other Insights**:
   - SVM excels in identifying negative sentiments but is less precise for positive sentiments.
   - Naive Bayes is effective but outperformed by Random Forest.

## Future Implications
- The insights gained will help in understanding customer preferences and improving product features based on feedback.
- The analysis can guide future marketing strategies and enhance customer engagement by addressing areas of dissatisfaction.
- Understanding whether positive or negative sentiments are associated with online purchasing preferences can guide marketing and sales strategies.
- Help gain insights into the factors driving consumer satisfaction and loyalty towards the brand.

