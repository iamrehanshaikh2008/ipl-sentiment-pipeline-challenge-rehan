Vectorizers
CountVectorizer

I selected CountVectorizer as a simple baseline because it represents text using word frequencies and allows comparison with more advanced vectorization methods.

HashingVectorizer

I selected HashingVectorizer because it is memory efficient, does not require storing a vocabulary, and provides a scalable alternative to traditional vectorizers.

TF-IDF Word Unigram

I selected TF-IDF Word Unigram because it captures the importance of individual words rather than just their frequency, making it one of the most widely used techniques for text classification.

TF-IDF Character 3–5 Grams

I selected TF-IDF Character 3–5 Grams because it captures character-level patterns and can better handle spelling variations and informal text.



Classifiers
Complement Naive Bayes

I selected Complement Naive Bayes because it is specifically designed for text classification and often performs well on sparse text features.

Multinomial Naive Bayes

I selected Multinomial Naive Bayes because it is a standard baseline classifier for text data and is computationally efficient.

Logistic Regression

I selected Logistic Regression because it is a strong linear classifier that generally provides reliable performance on text classification tasks.

LinearSVC

I selected LinearSVC because it is well suited for high-dimensional text data and is commonly used in natural language processing applications.





Combined Justification



I selected CountVectorizer, HashingVectorizer, TF-IDF Word Unigram, and TF-IDF Character 3–5 Grams to represent different approaches to text feature extraction. I selected Complement Naive Bayes, Multinomial Naive Bayes, Logistic Regression, and LinearSVC because they are widely used text classification algorithms with different learning strategies. Together, these methods provided a diverse and balanced set of pipelines for comparison.

