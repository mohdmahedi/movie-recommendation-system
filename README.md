# 🎬 Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange)
![Pandas](https://img.shields.io/badge/pandas-2.0.3-green)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> **AI & Data Science Internship Project** | Built using MovieLens 100K Dataset

---

## 📌 Project Overview

A complete Movie Recommendation System that implements **three recommendation techniques**:

| Approach | Technique | Accuracy |
|---|---|---|
| 🎯 Content-Based Filtering | Cosine Similarity on Genres | Moderate |
| 👥 Collaborative Filtering | User-User Similarity | Good |
| 🔬 SVD Matrix Factorization | Singular Value Decomposition | Best |

---

## 📊 Dataset

- **Source:** [MovieLens 100K](https://grouplens.org/datasets/movielens/100k/)
- **Ratings:** 100,000 ratings
- **Users:** 943 users
- **Movies:** 1,682 movies
- **Rating Scale:** 1–5 stars
- **Sparsity:** ~93.7%

> ✅ The notebook **automatically downloads** the dataset — no manual steps needed!

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Jupyter Notebook or JupyterLab

### Installation

**Step 1: Clone this repository**
```bash
git clone https://github.com/YOUR_USERNAME/movie-recommendation-system.git
cd movie-recommendation-system
```

**Step 2: Install dependencies**
```bash
pip install -r requirements.txt
```

**Step 3: Launch Jupyter Notebook**
```bash
jupyter notebook Movie_Recommendation_System.ipynb
```

**Step 4: Run All Cells**
- Click `Kernel` → `Restart & Run All`
- The dataset downloads automatically on first run

---

## 📁 Project Structure

```
movie-recommendation-system/
│
├── Movie_Recommendation_System.ipynb   # Main notebook (complete code)
├── requirements.txt                     # Python dependencies
├── README.md                            # This file
│
└── outputs/ (generated after running)
    ├── eda_plots.png                    # EDA visualizations
    ├── user_demographics.png            # User analysis
    ├── user_item_matrix.png             # Rating matrix heatmap
    ├── content_based_recommendations.png
    └── model_comparison.png             # RMSE comparison chart
```

---

## 🔍 Key Steps in the Notebook

1. **📥 Data Loading** — Auto-download and load MovieLens 100K
2. **🔍 EDA** — Rating distribution, genre analysis, user demographics
3. **🏗️ Matrix Building** — Create 943×1682 User-Item matrix
4. **🎯 Content-Based** — Genre cosine similarity recommendations
5. **👥 Collaborative Filtering** — User-user similarity recommendations
6. **🔬 SVD** — Matrix factorization with cross-validation
7. **📈 Evaluation** — RMSE & MAE comparison across all models

---

## 📈 Results

| Model | RMSE | MAE |
|---|---|---|
| Baseline (Global Mean) | ~1.12 | ~0.94 |
| Collaborative Filtering | ~1.03 | ~0.83 |
| SVD Matrix Factorization | **~0.94** | **~0.74** |

---

## 🛠️ Technologies Used

- **Python 3.8+**
- **pandas** — Data manipulation
- **numpy** — Numerical operations
- **scikit-learn** — Cosine similarity, train/test split, RMSE
- **scikit-surprise** — SVD matrix factorization
- **matplotlib** — Visualizations
- **seaborn** — Statistical plots

---

## 💡 Sample Usage

```python
# Content-Based: Find movies similar to Toy Story
recommendations = content_based_recommend('Toy Story', n=10)

# Collaborative Filtering: Recommend for User 1
cf_recs = collaborative_filter_recommend(user_id=1, n=10)

# SVD: Best recommendations for User 1
svd_recs = svd_recommend(user_id=1, n=10)
```

---

## 📚 References

- [MovieLens Dataset — GroupLens Research](https://grouplens.org/datasets/movielens/)
- [Surprise Library Documentation](https://surprise.readthedocs.io/)
- [Collaborative Filtering — Towards Data Science](https://towardsdatascience.com)

---

## 👤 Author

**Mohd Mahedi Bakali**  
Intern at **Codec Technologies**

---

*⭐ Star this repo if you found it helpful!*
