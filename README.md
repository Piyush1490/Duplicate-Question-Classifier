# Duplicate-Question-Classifier
Duplicate Question Classifier
This project focuses on identifying duplicate questions using advanced NLP techniques and machine learning models. The aim is to develop a system that accurately detects if two given questions are semantically identical, even if phrased differently. Such systems are critical for platforms like Quora or customer support portals, where redundant questions can reduce efficiency and clutter the platform.



Data Loading and Sampling:
The dataset is loaded using Pandas (train.csv), and a sample of 30,000 rows is taken for further processing.
https://www.kaggle.com/c/quora-question-pairs

Data Preprocessing:
It involves cleaning text by:
Expanding contractions (like converting "you're" to "you are").
Removing HTML tags using BeautifulSoup.
Removing punctuation using regex.
These steps suggest the goal is to normalize the text for comparison or analysis.

Advanced Feature Engineering:

Text Length: Extract features like word count, character length, and token counts from questions.
Word Overlap: Calculate the number of common and unique words between question pairs.
Stopword Analysis: Determine the ratio of common stopwords to total words.
Fuzzy Matching: Use fuzzywuzzy metrics (like token sort and set ratios) to capture word-level similarity.


Libraries Used:
Core Python libraries like numpy and pandas for data handling.
BeautifulSoup for HTML parsing.
Visualization tools (matplotlib).

Modeling & Evaluation:
RandomForestClassifier and XGBoost are employed for classification.
Achieved accuracy-
Random Forest: 78.4%
XGBoost: 79.2%

Future Work:
Implement advanced feature engineering (TF-IDF, word embeddings).
Experiment with different machine learning models (SVM, XGBoost).
Explore deep learning approaches (LSTM, BERT) for better performance.
