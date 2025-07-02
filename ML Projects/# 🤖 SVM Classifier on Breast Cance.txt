# 🤖 SVM Classifier on Breast Cancer Dataset

This project demonstrates the use of a **Support Vector Machine (SVM)** classifier to predict whether a tumor is malignant or benign using the **Breast Cancer Wisconsin dataset**. It is a classical binary classification task in machine learning.

---

## 📚 Dataset

- **Source:** `sklearn.datasets.load_breast_cancer()`
- **Features:** 30 numeric features related to cell nuclei
- **Target:** 
  - `0` = malignant  
  - `1` = benign  
- Total samples: 569

---

## 📌 Project Workflow

1. **Data Loading**
   - Used the breast cancer dataset from scikit-learn.

2. **Exploratory Data Analysis**
   - Viewed basic statistics and shape of the dataset.
   - Checked for missing values (none).

3. **Data Splitting**
   - Split into training and testing sets (80% train, 20% test).

4. **Feature Scaling**
   - Applied `StandardScaler` to normalize the feature values.

5. **Model Training**
   - Used `SVC()` from scikit-learn with default parameters.
   - Trained the model on the scaled training data.

6. **Evaluation**
   - Evaluated using **accuracy score** and **confusion matrix**.

---

## 📊 Results

| Metric             | Value     |
|--------------------|-----------|
| Training Accuracy  | ~98.9%    |
| Testing Accuracy   | ~96.4%    |
| Confusion Matrix   | `[[40, 3], [ 1, 70]]` |

✅ The model performs well on both training and test sets.

---

## 🛠️ Tools & Libraries Used

```python
Python
Jupyter Notebook
pandas
numpy
matplotlib
seaborn
sklearn
