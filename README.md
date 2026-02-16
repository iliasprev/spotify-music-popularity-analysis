# 🎵 Spotify Cross-Platform Streaming Analysis

## 📌 Executive Summary

This project analyses cross-platform engagement signals (Spotify playlists, TikTok, YouTube and Shazam) to determine which factors most strongly influence Spotify streaming performance.

Using statistical analysis and regression techniques, the results show that:

- Playlist reach is a key growth driver.
- Shazam counts are the strongest predictor of streaming volume.
- TikTok views alone do not reliably convert into streams.

---

## 🎯 Project Objectives

This project investigates whether cross-platform engagement metrics are statistically associated with Spotify streaming success.

Key questions explored:

- Does playlist exposure significantly increase Spotify streams?
- Does TikTok virality convert into streams?
- Is YouTube engagement a strong predictor?
- Does Shazam activity reflect real listener demand?
- Which platform shows the strongest statistical relationship?

---

## 🛠 Tools Used

- Python (Pandas, NumPy)
- Matplotlib
- Seaborn
- Tableau
- Jupyter Notebook
- Git & GitHub

---

## 📊 Methodology

### 1️⃣ Data Cleaning
- Removed duplicate records
- Converted numeric fields
- Handled missing values
- Created derived features (e.g. `release_year`)

### 2️⃣ Exploratory Data Analysis (EDA)
- Distribution analysis
- Outlier inspection
- Log transformations for skewed variables
- Correlation matrix analysis

### 3️⃣ Regression Analysis
- Built scatter plots with regression lines
- Applied log scaling where appropriate
- Compared R² values across platforms

### 4️⃣ Tableau Dashboard
- Interactive cross-platform comparison
- Visual exploration of streaming drivers

---

## 📊 Statistical Results

| Platform         | R² Value | Interpretation        |
|------------------|----------|------------------------|
| Playlist Reach   | 0.28     | Moderate relationship  |
| TikTok Views     | 0.003    | Very weak relationship |
| YouTube Views    | 0.22     | Moderate relationship  |
| Shazam Counts    | 0.48     | Strong relationship    |

---

## 🔎 Key Insights

### 🎧 Playlist Reach
Strong positive relationship. Tracks with higher playlist exposure tend to generate more Spotify streams.

### 🎥 TikTok
Statistically significant but practically weak. Viral views do not reliably translate into sustained streaming performance.

### 📺 YouTube
Moderate relationship. Cross-platform consistency appears to support streaming growth.

### 🔍 Shazam
Strongest predictor of streaming volume. Search behaviour reflects real listener intent and demand.

---

## 💡 Business Implications

- Playlist strategy remains the strongest driver of streaming growth.
- TikTok virality alone does not guarantee sustained streaming success.
- Listener intent (Shazam searches) may act as an early performance indicator.
- Multi-platform consistency outperforms single-platform spikes.

---

## 📂 Project Structure
```
spotify-music-popularity-analysis/
├── data/
│ ├── raw/
│ └── processed/
├── images/
│ └── dashboard_overview.png
├── notebooks/
│ ├── 01_data_loading_and_cleaning.ipynb
│ └── 02_spotify_eda.ipynb
├── tableau/
├── outputs/
└── README.md
```
---

## 📊 Tableau Dashboard

Below is the final cross-platform analysis dashboard:

![Spotify Dashboard](images/images/dashboard_overview.png)

---
## 👤 Author

**Ilias Prevyzis**  
Data Analyst | Python | SQL | Tableau
