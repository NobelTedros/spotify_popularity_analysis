# 🎵 Spotify Audio Feature Analysis — What's Associated with Song Popularity?

Exploratory data analysis and Ridge regression on 114,000+ Spotify tracks.  
Built to answer: **which audio characteristics are most strongly associated with a song's popularity?**

> **Note on causality:** All relationships in this analysis are correlational, not causal.  
> A feature being associated with popularity does not mean it drives popularity.

---

## Dataset

**Spotify Tracks Dataset** by Maharshi Pandya — [Kaggle link](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)

Contains audio features for ~114,000 tracks across 125 genres, including danceability, energy,
valence, tempo, loudness, acousticness, instrumentalness, and Spotify's popularity score (0–100).

---

## Tools Used

- **Python** — pandas, NumPy, SciPy, scikit-learn
- **Visualization** — Matplotlib, Seaborn
- **Statistics** — Pearson correlation, Ridge regression, train/test split, StandardScaler

---

## Key Findings

1. **Instrumentalness has the strongest negative association with popularity** — tracks with vocals dramatically outperform instrumentals across all genres.
2. **Acousticness is negatively associated with popularity** — produced, electric-sounding tracks score higher on average than acoustic ones.
3. **Danceability has a modest positive association** — more danceable tracks tend to score slightly higher, but the effect is weak.
4. **Audio features alone explain only ~7% of popularity variance (R² ≈ 0.07, RMSE ≈ 17.6)** — the remaining ~93% is driven by artist following, playlist placement, and marketing factors this dataset cannot capture. This is the most honest and interesting result in the project.

---

## How to Run

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/spotify-popularity-analysis.git
cd spotify-popularity-analysis
```

### 2. Download the dataset
- Go to: https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset
- Click **Download** (free Kaggle account required)
- Unzip the file — you'll get `dataset.csv`
- Place `dataset.csv` in the **same folder as the notebook**

### 3. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
```

### 4. Run the notebook
```bash
jupyter notebook spotify_popularity_analysis.ipynb
```
Then: **Kernel → Restart & Run All**

---

## Project Structure

```
spotify-popularity-analysis/
├── spotify_popularity_analysis.ipynb   # Main analysis notebook
├── README.md                           # This file
└── dataset.csv                         # Download from Kaggle — not included in repo
```

---

## Author

**Nobel Tedros** — Virginia Tech, B.S. Computational Modeling & Data Analytics, M.S. Applied Data Science
[LinkedIn](https://www.linkedin.com/in/nobel-tedros-b08044262)
