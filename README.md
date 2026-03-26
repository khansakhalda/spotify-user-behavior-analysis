# 🎧 Spotify User Behavior Analysis

## 📌 Background

The growth of music streaming platforms like Spotify generates large amounts of user data. However, user listening behavior is complex and difficult to interpret without proper analysis.

This project aims to analyze Spotify user behavior to identify patterns, segment users, and uncover relationships between music genres using machine learning techniques.

---

## 🎯 Objectives

* Analyze user listening behavior
* Identify music consumption patterns
* Segment users using clustering
* Discover genre relationships using association rules

---

## ⚙️ Methodology

* **Preprocessing**: Data cleaning, feature selection, and standardization
* **PCA**: Reduced 4 features into 2 components (51% variance explained)
* **Clustering**: K-Means with optimal K = 3
* **Association Rules**: Apriori algorithm (371 rules discovered)

---

## 📊 Results & Insights

### 🔹 User Segmentation

* **Cluster 0 – Efficient listeners**
  High number of songs with short listening time

* **Cluster 1 – Consistent listeners**
  Longer sessions with frequent access

* **Cluster 2 – Exploratory listeners**
  Highest listening time with diverse behavior

---

### 🔹 Genre Patterns

* Cluster 0 → Stable genre preferences
* Cluster 1 → Strong genre pair relationships
* Cluster 2 → Most diverse and complex genre combinations

---

### 🔹 Key Insight

This analysis is based on **301 Spotify users**, with no missing values or duplicate data, ensuring reliable results.

The results reveal three distinct user behavior segments:

* **🟢 Cluster 0 – Efficient listeners (116 users)**
  These users play the highest number of songs (~29 songs/day) despite having low listening time (~0.66 hours/day) and short sessions.
  👉 This indicates fast, efficient listening behavior, likely skipping tracks or preferring shorter songs.

---

* **🟠 Cluster 1 – Consistent listeners (109 users)**
  These users access Spotify most frequently (~2 times/day) and have the longest session duration (~0.45 hours), but listen to fewer songs (~11 songs/day).
  👉 This suggests focused and immersive listening habits.

---

* **🟣 Cluster 2 – Exploratory listeners (76 users)**
  These users have the highest listening time (~2.19 hours/day) with shorter sessions and moderate song counts.
  👉 This reflects dynamic behavior with strong exploration across different music genres.

---

In addition, **371 association rules** were discovered across clusters, revealing strong relationships between genres:

* Cluster 0 shows stable and predictable genre transitions
* Cluster 1 highlights consistent genre pairings
* Cluster 2 exhibits the most complex and diverse genre combinations

👉 These findings demonstrate the potential to build **behavior-aware and personalized recommendation systems**, tailored not only to user preferences but also to their listening patterns.

---

## 🛠️ Tools & Technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Mlxtend

---

## ✨ Author

Khansa Khalda – Machine Learning Final Project
