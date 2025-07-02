# 🎬 Movie Recommender System

This project demonstrates how to build a simple **content-based movie recommendation system** using Python. It recommends movies based on similarity of genres, keywords, cast, and other metadata.

---

## 📌 Project Highlights

- Used a dataset containing **movie metadata** (titles, genres, cast, overview, etc.)
- Cleaned and processed text data to extract meaningful features
- Combined multiple columns into a single "tags" column
- Applied **TF-IDF Vectorization** to convert text into numerical form
- Used **cosine similarity** to find and recommend similar movies

---

## 🧠 Techniques Used

- Text preprocessing (lowercasing, stemming)
- Feature engineering (merging relevant columns)
- Vectorization using `CountVectorizer`
- Cosine similarity matrix for recommendations

---

## 📊 Example Output

If you search for a movie like **"The Dark Knight"**, it might recommend:
- Batman Begins  
- The Dark Knight Rises  
- Man of Steel  
- Iron Man  

(All based on similarity in genre, cast, and description)

---

## 🔧 Libraries Used

```python
pandas
numpy
nltk
sklearn
