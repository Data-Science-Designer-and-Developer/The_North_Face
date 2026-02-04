Absolutely! Here’s the **full, ready-to-copy English version** of your README.md for CDSD:

---

# The North Face Product Catalog Analysis – CDSD Certification Project

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Pandas](https://img.shields.io/badge/Pandas-1.6-green) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2-yellow) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-ML-orange)

---

## 📌 Executive Summary

This project demonstrates **unsupervised machine learning applied to The North Face product catalog** to enhance e-commerce performance.
It focuses on:

* **Clustering products** by description similarity.
* **Recommending similar products** to increase conversion rates.
* **Topic extraction** to optimize catalog structure for better user navigation.

> Clean, reproducible, and structured notebooks for CDSD certification evaluation.

---

## 🎯 Objectives

1. **Cluster Analysis:** Identify coherent groups of products.
2. **Simple Recommender System:** Suggest similar products to users.
3. **Topic Modeling:** Extract latent topics for catalog optimization.

---

## 🗂 Repository Contents

| File                                | Purpose                                                       |
| ----------------------------------- | ------------------------------------------------------------- |
| `02-The_North_Face_ecommerce.ipynb` | Main analysis notebook                                        |
| `CDSD_Bloc4_TheNorthFace.ipynb`     | Certification-focused notebook                                |
| `README.md`                         | Project documentation                                         |
| `.gitignore`                        | Excludes unnecessary files/folders (`Old_Crap/`, checkpoints) |

---

## ⚙️ Methodology

**1. Data Preparation & Cleaning**

* Combine relevant text columns into a single `raw_text`.
* Clean and lemmatize using SpaCy (stopwords and punctuation removed).

**2. Feature Engineering**

* TF-IDF vectorization (unigrams + bigrams, top 20k features).

**3. Clustering**

* DBSCAN with cosine similarity to detect product clusters.
* Evaluate clusters using Silhouette Score.
* Visual interpretation using cluster distributions and word clouds.

**4. Recommender System**

* Recommends products within clusters; handles “noise” items globally.
* Based on cosine similarity of TF-IDF vectors.

**5. Topic Modeling**

* Latent Semantic Analysis (LSA) via TruncatedSVD.
* Top words and word clouds for each topic.

---

## ✅ Key Outcomes

* **Clusters**: Identified coherent product groups (e.g., outdoor gear, apparel).
* **Recommender**: Generates personalized suggestions for users.
* **Topics**: Revealed latent categories for potential catalog restructuring.

**Optional improvements:** KMeans clustering, NMF for more interpretable topics, or pure cosine similarity for fine-grained recommendations.

---

## 📖 How to Run

```bash
git clone https://github.com/Dreipfelt/The_North_Face.git
pip install -r requirements.txt
```

**Author:** (Dreipfelt)
