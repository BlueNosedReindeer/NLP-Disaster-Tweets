# NLP Disaster Tweets

This project was created as part of a Natural Language Processing course and submitted to the "NLP with Disaster Tweets" Kaggle competition. The goal was to build a model that classifies tweets as either referring to a real disaster or not. The dataset includes over 7,600 labeled tweets for training and about 3,200 for testing, with features like tweet text, keywords, and user-provided location data.

We used a Bidirectional LSTM model built with TensorFlow and Keras. Before training, tweets were cleaned by removing or replacing noisy elements like links, mentions, and hashtags, while preserving useful punctuation like exclamation points and question marks. We also merged the `keyword` field into the tweet text to enrich the input. The model architecture includes an embedding layer, a Bi-LSTM layer, and a couple of dense layers with dropout for regularization. It achieved around 84% validation accuracy and a 0.90 AUC score, with a public leaderboard F1 score of approximately 0.842.

In the future, we aim to fine-tune a lightweight transformer model such as DistilBERT, incorporate geolocation features, explore data augmentation techniques, and ensemble predictions from different models to further improve performance.

