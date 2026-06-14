# IPL Sentiment Analysis Project

## Project Summary

In this project, I explored different machine learning approaches for IPL sentiment classification. Instead of focusing on finding a single best-performing model, the goal was to identify a balanced set of vectorizers and classifiers that produced strong results while representing different text processing and learning techniques.

The project follows a complete machine learning workflow, including data loading, preprocessing, feature extraction, model training, evaluation, ranking, and result analysis.

---

## Objective

The objective of this project was to evaluate different text vectorization and classification techniques for sentiment analysis. Rather than selecting only the highest-performing model, the goal was to identify a balanced set of four vectorizers and four classifiers that produced strong results while representing different approaches to feature extraction and machine learning. This allowed a broader comparison of pipeline performance, efficiency, and diversity across multiple combinations.

---

## Dataset

The dataset consists of IPL-related text samples along with their corresponding sentiment labels. The dataset is loaded directly from a GitHub repository, making the project easy to reproduce.

### Preprocessing Steps

The following preprocessing steps were performed:

* Removed missing values
* Converted text to lowercase
* Removed extra whitespace
* Standardized text formatting
* Split the data using a 75:25 train-test ratio

```python
train_test_split(test_size=0.25, random_state=42)
```

---

## Selected Vectorizers and Classifiers

I selected CountVectorizer, HashingVectorizer, TF-IDF Word Unigram, and TF-IDF Character 3–5 Grams to compare different methods of converting text into numerical features. I chose Complement Naive Bayes, Multinomial Naive Bayes, Logistic Regression, and LinearSVC because they are commonly used in text classification and represent different machine learning approaches. By combining these vectorizers and classifiers, I was able to evaluate 16 different pipelines and compare their performance across the dataset.

### Vectorizers

* CountVectorizer
* HashingVectorizer
* TF-IDF Word Unigram
* TF-IDF Character 3–5 Grams

### Classifiers

* Complement Naive Bayes
* Multinomial Naive Bayes
* Logistic Regression (Balanced)
* LinearSVC

### Total Pipelines

4 Vectorizers × 4 Classifiers = 16 Pipelines

---

## Approach

For this project, I first loaded the IPL sentiment dataset from GitHub and cleaned the text data by standardizing the format and handling missing values. After that, I split the dataset into training and testing sets using a 75:25 ratio.

I then created 16 different machine learning pipelines by combining 4 vectorizers with 4 classifiers. Each pipeline was trained and evaluated using multiple performance metrics such as accuracy, F1 score, precision, and recall.

Finally, I compared the results, ranked the pipelines using a custom scoring system, and used the rankings to identify a diverse and effective set of vectorizers and classifiers for text classification.

---

## Evaluation Metrics

Each pipeline was evaluated using:

* Accuracy
* Macro F1 Score
* Weighted F1 Score
* Precision (Macro)
* Recall (Macro)
* Training Time
* Prediction Time
* Model Size

---

## Ranking Method

To compare pipelines fairly, a custom scoring system was used. The final ranking considered:

* Model performance
* Training and prediction speed
* Model size
* Overall simplicity and suitability

This helped identify methods that were not only accurate but also efficient and diverse in their approach.

---

## Results

All 16 pipeline combinations were trained and evaluated.

The notebook automatically:

* Trains all pipeline combinations
* Calculates evaluation metrics
* Generates performance rankings
* Displays a ranked results table
* Saves the results as CSV files

The rankings were then used to select a final set of vectorizers and classifiers that provided a good balance of performance, efficiency, and methodological diversity.

---

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run all cells from top to bottom.
3. The dataset will automatically be loaded from GitHub.
4. The notebook will train all 16 vectorizer-classifier combinations.
5. After training is complete, the results table will be displayed and saved as CSV files.
6. Review the rankings and compare the performance of the different approaches.

No manual changes are required—simply run the notebook and wait for all cells to finish executing.

---

## Conclusion

This project compared multiple vectorizer-classifier combinations for IPL sentiment classification. The focus was not only on performance but also on selecting a diverse set of techniques that represented different approaches to text representation and classification. The final selection of four vectorizers and four classifiers provided a balanced mix of simple, efficient, and advanced methods, allowing meaningful comparison across 16 pipeline combinations.
