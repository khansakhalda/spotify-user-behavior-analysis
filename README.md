# 🎧 Spotify User Behavior Analysis

## 📌 Background

The rapid growth of music streaming platforms such as Spotify has generated large amounts of user interaction data. Understanding user listening behavior is crucial for improving recommendation systems, enhancing user experience, and supporting data-driven decision making.

However, user behavior is often complex and varies significantly between individuals. Without proper analysis, it is difficult to identify meaningful patterns in how users consume music.

This project aims to analyze Spotify user behavior using machine learning techniques to uncover hidden patterns, segment users, and explore relationships between music genres.

---

## 🎯 Objectives

* Analyze Spotify user listening behavior
* Identify patterns in music consumption
* Segment users into distinct groups using clustering
* Discover relationships between music genres using association rule mining
* Provide insights to support recommendation systems

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Loaded dataset from CSV file
* Checked for missing values and duplicates (none found)
* Selected key numerical features:

  * Daily listening time
  * Average session duration
  * Daily access frequency
  * Number of songs played
* Standardized data using **StandardScaler**

---

### 2. Dimensionality Reduction (PCA)

* Applied **Principal Component Analysis (PCA)**
* Reduced 4 features into 2 components (PC1 & PC2)
* Explained variance:

  * PC1: 26%
  * PC2: 25%
  * Total: 51%

👉 PCA helps simplify data structure and enables visualization of user distribution.

---

### 3. Clustering (K-Means)

* Used **Elbow Method** and **Silhouette Score**
* Optimal number of clusters: **K = 3**
* Users were grouped based on behavioral similarity

---

### 4. Association Rule Mining

* Applied **Apriori algorithm** using Mlxtend
* Generated **371 association rules**
* Analyzed relationships between music genres within each cluster

---

## 📊 Results & Insights

### 🔹 User Segmentation

#### 🟢 Cluster 0 – Efficient Listeners

* Low listening time (~0.66 hours/day)
* Short sessions (~0.27 hours)
* Low access frequency (~1.11 times/day)
* Highest number of songs (~29 songs/day)

👉 Insight:
Users consume many songs in a short time, indicating efficient and fast listening behavior.

---

#### 🟠 Cluster 1 – Consistent Listeners

* Low listening time (~0.65 hours/day)
* Longest sessions (~0.45 hours)
* Highest access frequency (~2 times/day)
* Lowest number of songs (~11 songs/day)

👉 Insight:
Users prefer longer, focused listening sessions and consistent usage patterns.

---

#### 🟣 Cluster 2 – Exploratory Listeners

* Highest listening time (~2.19 hours/day)
* Short sessions (~0.18 hours)
* Moderate access frequency
* Moderate number of songs

👉 Insight:
Heavy users who explore various genres with dynamic listening behavior.

---

### 🔹 Genre Association Patterns

* Total rules discovered: **371 rules**

**Cluster 0**

* Strong, stable genre relationships
* Example: *blues, reggae → indie*

👉 Users have predictable music preferences

---

**Cluster 1**

* Strong genre pair relationships
* Example: *jazz → hip hop*

👉 Users prefer consistent genre combinations

---

**Cluster 2**

* Most complex and diverse rules (193 rules)
* Many high-confidence relationships

👉 Users explore diverse and non-mainstream genre combinations

---

### 🔹 Key Insight

This project reveals that Spotify users can be categorized into three behavioral types:

* Efficient listeners (short & high-volume consumption)
* Consistent listeners (long & focused sessions)
* Exploratory listeners (diverse & intensive usage)

Additionally, genre associations provide valuable insights for building more personalized and intelligent recommendation systems.

---

## 🛠️ Tools & Technologies

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Mlxtend

---

## ✨ Author

Khansa Khalda – Machine Learning Final Project
