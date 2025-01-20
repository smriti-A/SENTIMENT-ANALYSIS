# SENTIMENT-ANALYSIS

**COMPANY**: CODETECH IT SOLUTIONS

**NAME**: SMRITI KAUSHIK

**INTERN ID**: CT08JGJ

**DOMAIN**: DATA ANALYTICS

**BATCH DURATION**: JAN 5TH,2025 TO FEB 5TH,2025

**MENTOR NAME**: Neela Santhosh Kumar 

**DESCRIPTION**: This Python script performs sentiment analysis on Twitter data stored in a CSV file, classifying each tweet's emotional tone as positive, negative, or neutral. This type of analysis is crucial for understanding public opinion on various topics, tracking brand perception, and extracting valuable insights from social media conversations.  

Key Libraries and Their Functions:

pandas: This library is the cornerstone of data manipulation in Python. Here, pandas is used to:  

Efficiently read the CSV file containing the tweet data into a structured table-like format called a DataFrame.   Extract the column labeled "TWEET CONTENT," which holds the actual tweet text, and convert it into a standard Python list. This list format is essential for compatibility with the sentiment analysis tool. re (Regular Expressions): This library provides powerful tools for pattern matching and text manipulation. It's employed for essential text preprocessing steps:  
Removal of URLs (web addresses): URLs rarely contribute to sentiment and can introduce noise. Removal of user mentions (@usernames): These are references to other users and generally don't reflect the sentiment of the tweet itself. Removal of hashtags (#hashtags): While hashtags can sometimes provide context, they are often used for categorization and can distract from the core sentiment. Standardization of text: Non-alphanumeric characters are removed, and the text is converted to lowercase. This standardizes the text, making it easier for the sentiment analyzer to recognize words regardless of capitalization or punctuation variations. nltk (Natural Language Toolkit): This is a leading library for natural language processing (NLP). The script uses nltk and, specifically, the VADER (Valence Aware Dictionary and sEntiment Reasoner) lexicon for sentiment analysis.  

**OUTPUT**
![Image](https://github.com/user-attachments/assets/8d7096f8-e9de-4c9f-9f99-1cf5ce56d6df)

VADER Lexicon Download: nltk.download('vader_lexicon') ensures the VADER lexicon, a dictionary of words and their associated sentiment scores, is downloaded and available for use. Sentiment Analysis: The SentimentIntensityAnalyzer class from nltk.sentiment.vader is instantiated to create a sentiment analyzer object. This object's polarity_scores() method is used to calculate sentiment scores for each tweet. Script Execution Process:
Setup and Data Input: The necessary libraries are imported, and the VADER lexicon is downloaded. The script then attempts to read the CSV file into a pandas DataFrame. Crucially, error handling using try...except blocks is implemented to manage potential FileNotFoundError.

OUTPUT:
