# 📱 SMS Spam Detection using Machine Learning

This project demonstrates how to classify SMS messages as **spam** or **ham** (non-spam) using basic NLP techniques and a Naive Bayes classifier. It’s a beginner-friendly machine learning project focused on text classification.

---

## 🧠 Project Goals

- Understand the workflow of text classification.
- Apply preprocessing techniques to clean raw SMS data.
- Convert text into numerical features using **TF-IDF Vectorization**.
- Train and evaluate a **Multinomial Naive Bayes model**.

---

## 🗂️ Dataset Info

- Source: SMS Spam Collection dataset
- Format: Tab-separated file with two columns:
  - `label`: Indicates "ham" or "spam"
  - `text`: The actual message content

---

## 🔧 Steps Performed

1. **Data Loading**
   - Imported dataset using `pandas`
   - Checked for null values and data imbalance

2. **Preprocessing**
   - Converted all text to lowercase
   - Removed special characters, punctuation, and stopwords
   - Applied stemming using `PorterStemmer`
   - Created a clean new column `transformed_text`

3. **Feature Extraction**
   - Used `TfidfVectorizer` with a max feature limit of 3000
   - Transformed text data into numerical vectors

4. **Modeling**
   - Applied `MultinomialNB` (Naive Bayes)
   - Trained model on training set (80%)
   - Evaluated with accuracy score and confusion matrix

---

## 📊 Results

| Metric           | Value   |
|------------------|---------|
| Accuracy Score   | ~95%    |
| Confusion Matrix | [[965,  10], [ 27, 147]] |

> Great precision and recall for spam detection with Naive Bayes.

---

## 🛠️ Libraries Used

```python
pandas
numpy
matplotlib
seaborn
nltk
sklearn
