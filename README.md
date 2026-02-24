# 🎵 Spotify Cross-Platform Streaming Analysis

> 📌 End-to-end data analysis project:  
> Data cleaning → Exploratory analysis → Statistical modelling → Business insights

---

## 📚 Table of Contents

- [Executive Summary](#-executive-summary)
- [Project Objectives](#-project-objectives)
- [Data Source](#-data-source)
- [Tools Used](#-tools-used)
- [Methodology](#-methodology)
- [Statistical Results](#-statistical-results)
- [Key Insights](#-key-insights)
- [Final Insight](#-final-insight--what-drives-top-streaming-performance)
- [Project Structure](#-project-structure)
- [Notebooks](#-notebooks)
- [Tableau Dashboard](#-tableau-dashboard)
- [Author](#-author)

---

## 📌 Executive Summary

This project analyses cross-platform engagement signals (Spotify playlists, TikTok, YouTube and Shazam) to determine which factors are statistically associated with Spotify streaming performance.

Using descriptive statistics, correlation analysis, and regression modelling, the results indicate:

- Playlist reach is strongly associated with higher streaming volume.
- Shazam counts show the strongest explanatory relationship with streams.
- YouTube engagement demonstrates a moderate relationship.
- TikTok views alone do not reliably convert into sustained streams.
- Sustained multi-platform exposure is more consistent than single-platform spikes.

---

## 🎯 Project Objectives

This project investigates whether cross-platform engagement metrics are statistically associated with Spotify streaming success.

Key questions explored:

- Does playlist exposure relate to higher Spotify streams?
- Does TikTok virality convert into measurable streaming growth?
- Is YouTube engagement a reliable predictor?
- Does Shazam activity reflect real listener demand?
- Which platform shows the strongest statistical relationship?

---

## 📁 Data Source

Dataset: **Most Streamed Spotify Songs 2024**

The dataset contains:

- 4,600 tracks  
- 29 variables  
- Cross-platform engagement metrics  
- Playlist exposure indicators  
- Streaming counts  
- Listener search behaviour signals  

---

## 🛠 Tools Used

- Python (Pandas, NumPy)
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Tableau
- Git & GitHub

---

## 📊 Methodology

### 1️⃣ Data Cleaning  
➡ Implemented in:  
[01_data_loading_and_cleaning_CLEANED.ipynb](./notebooks/01_data_loading_and_cleaning_CLEANED.ipynb)

- Removed duplicate records (kept highest streamed version)
- Converted numeric fields from string format
- Standardised column naming (snake_case)
- Preserved missing values for transparency
- Converted date columns
- Exported cleaned dataset for Tableau

---

### 2️⃣ Exploratory Data Analysis (EDA)  
➡ Implemented in:  
[02_spotify_eda.ipynb](./notebooks/02_spotify_eda.ipynb)

- Distribution analysis
- Log transformations for skewed variables
- Pearson correlation analysis
- Linear regression modelling
- R² comparison across platforms
- Descriptive Top 10 vs overall group comparison

---

## 📊 Statistical Results

| Platform         | R² Value | Interpretation        |
|------------------|----------|------------------------|
| Shazam Counts    | ~0.53    | Strong relationship    |
| Playlist Reach   | ~0.38    | Moderate relationship  |
| YouTube Views    | ~0.22    | Moderate relationship  |
| TikTok Views     | ~0.001   | Very weak relationship |

R² represents the proportion of variance in Spotify streams explained by each individual platform metric in a simple linear regression model.

---

## 🔎 Key Insights

### 🎧 Playlist Reach
Strong positive association. Tracks with higher playlist exposure tend to generate significantly more Spotify streams.

### 📺 YouTube Engagement
Moderate relationship. Consistent cross-platform presence supports streaming growth.

### 🎥 TikTok
Statistically weak linear relationship. Viral views do not consistently translate into sustained streaming performance.

### 🔍 Shazam Activity
Strongest explanatory variable. Search behaviour reflects genuine listener intent and demand.

---

## 📈 Final Insight — What Drives Top Streaming Performance

A descriptive comparison between the Top 10 highest streamed tracks and the overall dataset shows substantially higher average exposure across all major platforms.

Top-performing tracks demonstrate consistently higher:

- Average Spotify streams  
- Playlist reach  
- TikTok exposure  

This comparison reflects group mean differences and does **not** imply causation, probability, or linear impact.

Overall findings suggest that sustained multi-platform exposure — particularly strong playlist placement and listener search behaviour (Shazam activity) — is closely associated with higher streaming performance.

However, correlation does not imply causation. Exposure may amplify already strong-performing tracks rather than directly cause success.

---

```

## 📂 Project Structure
spotify-music-popularity-analysis/
│
├── data/
│ ├── raw/
│ └── processed/
│
├── notebooks/
│ ├── 01_data_loading_and_cleaning_CLEANED.ipynb
│ └── 02_spotify_eda.ipynb
│
├── images/
│ └── dashboard_overview.png
│
├── tableau/
├── outputs/
└── README.md

```
---

## 📓 Notebooks

- 🔹 [01 — Data Loading & Cleaning](./notebooks/01_data_loading_and_cleaning_CLEANED.ipynb)
- 🔹 [02 — Exploratory Data Analysis](./notebooks/02_spotify_eda.ipynb)

Each notebook is documented and can be run sequentially.

---

## 📊 Tableau Dashboard

![Spotify Dashboard](./images/images/dashboard_overview.png)

---

## 👤 Author
**Ilias Prevyzis**  
Data Analyst | Python | SQL | Tableau