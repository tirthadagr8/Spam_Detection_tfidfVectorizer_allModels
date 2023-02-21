# Spam_Detection_tfidfVectorizer_allModels

This model distinguishes between spam and ham messages. The model first does necessary pre-processing on the text messages in the data, that is, removing special characters, single characters, lemmatizing the words using stopwords. Then using TFIDF Vectorizer, the processed text data is used to form a matrix of TF-IDF features.

(Term Frequency: (Number of repitition of words in a sentence)/(Number of words) | Inverse Document Frequency: log((Number of Sentences)/(Number of Sentences containing that word))

Now this matrix is used to split training and test data. Now, to avoid unbalanced data, we are creating artificial data using SMOTE.

Then XGBoost, Naive Bayes, SVC, Decision Tree, Random Forest, Logistic Regression models are tested to find the model with highest accuracy.
