# 🎬 Netflix Titles Clustering Project

This project explores the use of **unsupervised machine learning** to cluster Netflix titles based on content metadata. The aim is to group similar titles and uncover patterns that can be used for **content recommendation**, **user segmentation**, and **marketing strategies**.

---

## 📌 Project Objective

> Group Netflix titles (Movies & TV Shows) into meaningful clusters based on content features using clustering algorithms and PCA visualization.

---

## 🗂️ Dataset

The dataset includes publicly available Netflix metadata, with the following key fields:

- `title`, `type` (Movie or TV Show)
- `release_year`, `rating`, `duration`
- `genres` (listed as "listed_in")
- `country`, `description`

---

## 🛠️ Techniques Used

### 🔹 Preprocessing
- Handled missing values and duplicates
- One-hot encoded categorical features (e.g., genres, country)
- Transformed `duration` to numeric form
- Combined multi-label features into vectors

### 🔹 Dimensionality Reduction
- **PCA (Principal Component Analysis)** was used to reduce high-dimensional feature space to 2D for visualization.

### 🔹 Clustering Algorithms
- **K-Means Clustering**
- **Hierarchical Agglomerative Clustering**
- **DBSCAN (Density-Based Spatial Clustering)**

---

## 📊 Visual Outputs

Each clustering algorithm was visualized after PCA dimensionality reduction:
- **KMeans**: Clearly separated clusters, effective for compact groups.
- **Hierarchical**: Balanced results with interpretable structure.
- **DBSCAN**: Good for identifying noise and irregular group shapes, but grouped most points into one cluster.

---

## 🔍 Key Outcomes

- **KMeans and Hierarchical** yielded 4–5 clear clusters, which corresponded to genre-duration-release year combinations.
- **DBSCAN** struggled due to high-dimensional sparsity and labeled most data as a single cluster.
- These clusters can be interpreted for:
  - Content-based recommendation systems
  - Targeted promotions for user segments
  - Insights into content acquisition strategies

---

## 💼 Business Impact

| Application Area      | Value Generated                                     |
|-----------------------|------------------------------------------------------|
| 📽️ Recommendation     | Suggest similar titles based on content cluster     |
| 📈 Marketing           | Segment users by preferences and tailor campaigns   |
| 📊 Portfolio Analysis | Understand gaps in content offerings per cluster     |

---

