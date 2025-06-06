# Book Recommender System

A personalized book recommender system that suggests books to users based on their reading preferences and past ratings, using collaborative filtering techniques on the Book Crossing dataset.

---

## 📂 Project Structure
```book-recommender-system/
│
├── Data/
│ ├── Books.csv
│ ├── Ratings.csv
│ ├── Users.csv
│
├── Notebooks/
│ ├── 01_data_preparation.ipynb
│ ├── 02_book_recommendation_engine.ipynb
│
├── Outputs/
│ ├── user_book_ratings.libsvm
│ ├── Top5_Book_Recommendations.csv
│
├── Reports/
│ ├── Book_Recommender_Report.docx
│
├── .gitignore
└── README.md
```

---

## 📘 Dataset Description

This project uses the [Book Crossing Dataset](https://www.kaggle.com/datasets/somnambwl/bookcrossing-dataset?resource=download) which includes:

- **Books.csv** – Metadata such as title, author, and ISBN  
- **Users.csv** – User IDs and demographics  
- **Ratings.csv** – User ratings of books on a 0–10 scale  

Total:  
📚 270,000+ books  
👥 270,000+ users  
⭐ 1 million+ ratings

---

## 🔍 Objective

To build a recommender system that:
- Understands user preferences from prior ratings
- Computes similarity between users using collaborative filtering
- Recommends top 5 books that a user hasn’t read yet but is likely to enjoy

---

## ⚙️ Methodology

1. **Data Cleaning & LIBSVM Preparation**  
   [`01_data_preparation.ipynb`](Notebooks/01_data_preparation.ipynb)  
   - Removes invalid entries  
   - Filters non-positive ratings  
   - Converts to sparse matrix and LIBSVM format  

2. **Collaborative Filtering Engine**  
   [`02_book_recommendation_engine.ipynb`](Notebooks/02_book_recommendation_engine.ipynb)  
   - Builds user-user similarity matrix (Cosine similarity)  
   - Finds top 10 nearest neighbors per user  
   - Generates 5 book recommendations per user  
   - Outputs results to CSV  

---

## 📁 Outputs

- `user_book_ratings.libsvm`: Sparse matrix in LIBSVM format  
- `Top5_Book_Recommendations.csv`: Final output with recommended books and scores  

---

## 🧾 Report

A clean summary of project objectives, methodology, and outcomes is available here:  
[`Book_Recommender_Report.docx`](Reports/Book_Recommender_Report.docx)

---

## 🧑‍💻 Technologies Used

- Python (Pandas, NumPy, Scikit-learn, SciPy)
- Jupyter Notebooks
- Cosine Similarity (Collaborative Filtering)
- LIBSVM Format

---

## 👨‍🎓 Course

This academic project was developed under the course **IFT 511: Analyzing Big Data (Spring 2025)** at **Arizona State University**.

---

## 📝 Authors

Taljinder Singh 


