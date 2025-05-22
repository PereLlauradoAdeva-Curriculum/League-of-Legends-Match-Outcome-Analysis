# 🧠 League of Legends Match Outcome Analysis

This project dives into a dataset of over **100,000 ranked League of Legends matches** to understand which in-game factors contribute most to winning. By applying data cleaning, feature engineering, and correlation analysis, we uncover the most decisive actions in a match.

---

## 📊 Project Overview

We aimed to identify what events during a match — like securing dragons, pushing towers, or gaining gold leads — most strongly correlate with victory.

The workflow followed:
- **Data Cleaning:** Removal of null rows and irrelevant features
- **Feature Selection:** Kept numerical and binary indicators of gameplay (kills, deaths, turrets, objectives, etc.)
- **Correlation Analysis:** Calculated Pearson correlations between all features and the target variable `hasWon`
- **Visualization:** Built a heatmap to display the most impactful features in an intuitive way

---

## 🔍 Key Insights

From the heatmap, we found:

✅ **Strong positive correlation** with victory:
- Gold difference (`goldDiff`)
- Number of kills (`kills`) and assists (`assists`)
- Destroyed turrets (especially `destroyedInnerTurret`)

❌ **Strong negative correlation**:
- Lost inhibitors (`lostInhibitor`)
- Lost Baron Nashor (`lostBaronNashor`)

These findings align well with competitive strategies, highlighting the value of early pressure and map control.

---

## 🛠️ Tools Used

- Python
- Jupyter Notebook
- `pandas`, `numpy`
- `seaborn`, `matplotlib`

---

## 📁 Files Included

- `lol_ranked_games.csv`: Preprocessed match dataset compressed 
- `CasKaggle.ipynb`: Jupyter notebook with full analysis  
- `output.png`: Heatmap showing feature correlation with victory  

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/LoL-Match-Analysis.git
   cd LoL-Match-Analysis
