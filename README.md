# Book Recommender System: Content-Based vs. Collaborative Filtering

This project implements and compares two book recommendation approaches—Content-Based Filtering and Collaborative Filtering (SVD)—using the Book-Crossing dataset.

---

## 📚 Project Overview

- **Goal:**  
  Design and evaluate a recommender system pipeline using real-world book data.
- **Dataset:**  
  [Book-Crossing Dataset (Kaggle)](https://www.kaggle.com/datasets/saurabhbagchi/books-dataset)
- **Team Members:**  
  Shadi Farzankia 107209  
  Shruti Pashine 106369  
  Dharampal Singh 106316

---

## 🚀 Workflow

1. **Data Loading & Preprocessing:**  
   - Load books, ratings, and users data.
   - Clean and merge datasets, handle missing values and outliers.

2. **Exploratory Data Analysis (EDA):**  
   - Visualize distributions, check for anomalies, and understand feature relationships.

3. **Recommendation Approaches:**  
   - **Content-Based Filtering:** Uses book metadata (title, author, publisher) with TF-IDF and cosine similarity.
   - **Collaborative Filtering (SVD):** Uses user-book ratings and matrix factorization (Surprise SVD).

4. **Evaluation:**  
   - Precision@5 (Hit Rate) for both methods.
   - RMSE for SVD.

5. **Comparison & Discussion:**  
   - Compare strengths, weaknesses, and visualize results.

---

## 🗂️ Data

Place the following files in a `data/` directory:
- `books.csv`
- `ratings.csv`
- `users.csv`

---

## 🛠️ How to Run

1. Clone this repository.
2. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3. Open the notebook (`Code/RecommenderSytems.ipynb`) in Jupyter or VS Code.
4. Run all cells in order.

---

## 📊 Key Findings

- **Content-Based Filtering:**  
  - Interpretable, works for new/unpopular books, higher hit rate.
- **SVD Collaborative Filtering:**  
  - More accurate in rating prediction (lower RMSE), more personalized, but needs enough user-book interactions.

---

## ⚠️ Limitations & Future Work

- Data sparsity and cold-start issues for collaborative filtering.
- Evaluation for SVD is limited to a sample of users for computational reasons.
- Future work: hybrid models, more features, deep learning approaches.

---

## 📎 Authors

Shadi Farzankia, Shruti Pashine, Dharampal Singh

---

**Dataset:** [Book-Crossing Dataset (Kaggle)](https://www.kaggle.com/datasets/saurabhbagchi/books-dataset)