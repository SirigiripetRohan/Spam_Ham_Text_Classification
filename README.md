# Spam_Ham_Text_Classification
Classifying the real time text into spam or normal messages (text).
################################################ SPAM-HAM TEXT CLASSIFICATION##########################################################
1. Classify the messages in to Ham or Spam.
2. Dataset consists of 5026 records and columns as Message and Category.
3.Out of 5026 rows , 3235 rows are null for both columns (Message and Category) . Removed these records.
4.Now total records are 1790, out of these 65 records contain null categories for messages. So I am considering 65 records as test dataset.
5.We are considering out of 1725 records 1552 rows for training and 173 records (10 percentage) for Validation. 
6. Now we need to clean the text before processing it. For that we considered following operations like removing punctuations, stop words , URL'S, and many other special symbols as said below.
7. Lemmatizing the words to their root form.
8.Used Spacy nlp library for converting text to embeddings (Spacy pretrained-model en_vectors_web_lg).
9. Could see the target variable is imbalanced , used smoting technique to balance target varaible
9. Applied various machine learning algorithms (Linear SVC, Random forest) on features(embeddings) got from spacy.
10. Could see Random forest perfomed well and got fair results.
