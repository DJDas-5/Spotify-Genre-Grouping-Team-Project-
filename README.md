# 🎵 Spotify Genre Grouping using Machine Learning

##  Overview
This project groups Spotify songs into clusters based on their audio features using unsupervised machine learning.<br>
It uses K-Means clustering along with dimensionality reduction techniques like PCA and t-SNE to identify patterns in music genres.

---

##  Features
- Data Cleaning & Preprocessing<br>
- Feature Selection & Scaling<br>
- Dimensionality Reduction using PCA & t-SNE<br>
- K-Means Clustering<br>
- Hyperparameter Tuning using Elbow Method & Silhouette Score<br>
- Outlier Detection & Removal using Silhouette Scores<br>
- Cluster Visualization using Plotly<br>

---

##  Dataset
- Dataset: Spotify Songs Dataset<br>
- Focused Genres:<br>
  - Pop<br>
  - Rap<br>
  - Rock<br>
  - Latin<br>
  - R&B<br>
  - EDM<br>

- Audio Features Used:<br>
  - Danceability<br>
  - Energy<br>
  - Loudness<br>
  - Speechiness<br>
  - Acousticness<br>
  - Instrumentalness<br>
  - Liveness<br>
  - Valence<br>
  - Tempo<br>

---

##  Workflow

### 1️⃣ Data Cleaning
- Removed missing values and duplicates<br>
- Filtered only selected genres :contentReference[oaicite:0]{index=0}  

### 2️⃣ Feature Scaling
- StandardScaler used to normalize features :contentReference[oaicite:1]{index=1}  

### 3️⃣ Dimensionality Reduction
- PCA used to retain 95% variance<br>
- t-SNE used for better visualization :contentReference[oaicite:2]{index=2}  

### 4️⃣ Clustering
- K-Means clustering applied<br>
- Tested multiple values of k (2–20) :contentReference[oaicite:3]{index=3}  

### 5️⃣ Hyperparameter Tuning
- Elbow Method (WCSS)<br>
- Silhouette Score for best cluster selection :contentReference[oaicite:4]{index=4}  

### 6️⃣ Outlier Removal
- Removed poorly clustered points (negative silhouette scores)<br>
- Improved clustering performance :contentReference[oaicite:5]{index=5}  

### 7️⃣ Final Clustering
- Re-trained K-Means on cleaned dataset<br>
- Visualized clusters using Plotly :contentReference[oaicite:6]{index=6}  

---

##  Model Details
- Algorithm: K-Means Clustering<br>
- Optimal Clusters (k): 2–3 (varies by method)<br>
- Evaluation Metric: Silhouette Score<br>

- Initial Silhouette Score: ~0.19<br>
- Improved Score after cleaning: ~0.23–0.37 :contentReference[oaicite:7]{index=7}  

---

##  Results
- Improved clustering quality after removing outliers<br>
- Clear separation of music groups in visualization<br>
- t-SNE provided better cluster separation than PCA<br>


---

## ⚙️ Technologies Used
- Python<br>
- Pandas<br>
- NumPy<br>
- Matplotlib<br>
- Seaborn<br>
- Plotly<br>
- Scikit-learn<br>

---
## Future Improvements
Use Deep Learning clustering methods<br>
Try DBSCAN / Hierarchical Clustering<br>
Deploy as a web app<br>
Real-time music recommendation system<br>
