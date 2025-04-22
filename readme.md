# 🎶 TLAB: Unsupervised Music Recommendation Algorithm 🎶

This repository presents an unsupervised learning pipeline designed to cluster songs by thematic content, enabling personalized music recommendations without relying on labeled user data. The goal is to enhance content delivery through scalable, intelligent user modeling.

## 📊 Project Overview 

This project implements an end-to-end clustering workflow using scikit-learn and real-world lyric data, following the typical stages of an unsupervised machine learning pipeline.

The objective is to cluster unlabeled songs based on lyrical themes, forming the basis of a recommendation system that can suggest music without prior user labels. The workflow includes:

### Exploratory Data Analysis (EDA) 
- Evaluated theme distributions across songs
- Checked for missing data and structural issues
- Analyzed potential correlations between lyrical categories
### Preprocessing & Scaling – to prepare thematic features for modeling
- Standardized thematic variables using StandardScaler
- Avoided dimensionality reduction (e.g., PCA) to preserve interpretability of theme clusters
### Clustering & Evaluation – to group songs using KMeans and assess cluster quality
- Used KMeans to identify natural groupings within the dataset
- Optimized cluster count using:
Elbow Method and Silhouette Score
### Interpretation & Reporting – to analyze cluster traits and surface meaningful recommendations
- Labeled and analyzed clusters based on theme prominence
- Compared representative tracks per cluster to assess lyrical patterns (e.g: “Low-Obscene,” “Romantic,” etc.)



## 🗂 Dataset

Lyrically analyzed songs, each annotated with quantified scores for themes

📥 Download the dataset
[Music Dataset](https://drive.google.com/file/d/1oGoUawIeH--KED4sB2MFyzBq90GppNnG/view?usp=sharing).

### Correlation Heat Map based on Thematic Colunns 
🔗 Correlation Analysis

A heatmap visualization was used to assess potential multicollinearity between themes. 
![alt text](image.png)
Result: No strong correlations—positive or negative—were found among the thematic categories. This supports the clustering approach, as songs are not easily grouped by simple co-occurrence of lyrical traits.


### Top Song Genres 
![alt text](image-1.png)
---
🎶


