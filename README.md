# Twitter Sentiment Analysis Using Machine Learning

This project explores various sentiment analysis models applied to Twitter data to classify tweets as **positive**, **negative**, or **neutral** using advanced machine learning techniques and feature engineering.

## Project Overview

The goal is to develop and benchmark sentiment classifiers that can analyze Twitter data effectively, enabling deeper insights into public opinions and emotions expressed in tweets. *Applications include brand monitoring, market research, and social media analytics.*

## Approach & Pipeline

### Dataset

- Tweets collected via the Twitter API, sometimes automatically labeled using emojis or hashtags.
- Data is **preprocessed** by:
  - Removing URLs, hashtags, mentions, and punctuation
  - Replacing emojis with their described emotions
  - Removing stop words and correcting spelling
  - Filtering out non-English tweets

### Feature Extraction

- Extraction of:
  - **Unigrams, bigrams, and n-grams** (word frequency and presence)
  - **Part-of-speech (POS) tags** (adjectives, adverbs, verbs, nouns)
  - **Opinion words** and sentiment-related phrases
  - **Negation detection** and syntactic patterns
  - **Hashtags** and **emoji-based sentiment markers**

### Models Evaluated

- **Naive Bayes** (unigram, bigram, and polynomial versions)
- **Maximum Entropy (MaxEnt)**
- **Support Vector Machines (SVM)**
- **Stochastic Gradient Descent (SGD)** on streaming data
- **Tree-based models** and **K-Nearest Neighbors (KNN)** for hashtag-focused sentiment

### Machine Learning Pipeline

1. Data preprocessing and cleaning
2. Feature vector construction using selected features
3. Train-test split for supervised classification
4. Model training with hyperparameter tuning
5. Evaluation using accuracy, precision, recall, and confusion matrices

### Sentiment Classification Levels

- **Document-level:** Classifies entire tweets
- **Sentence-level:** Classifies individual sentences (when applicable)
- **Aspect-level:** Detects sentiment about specific entities or features within the text

## Results

- **Naive Bayes classifiers** provide strong baselines and show good performance on Twitter datasets.
- **SVM models** often outperform Naive Bayes when enhanced features are incorporated.
- Combining features (POS tags, hashtags, sentiment lexicons) results in higher classification accuracy.
- **SGD** performs well on streaming Twitter data when appropriately tuned.
- **Tree-core and syntactic models** show promise by leveraging sentence structure.

## Model Limitations & Future Work

- **Tweets are short and context-limited**, which can restrict the effectiveness of complex models like bidirectional LSTM or BERT.
- **Challenges:** Handling spam, multilingual content, and sarcasm in tweets.
- Feature engineering and **hybrid model ensembles** could further improve performance.
- Future work might explore **contextual embedding models** for enhanced sentiment detection.
