# 🎮 Video Game Price vs Quality Analysis

An exploratory data analysis examining whether higher-priced video games deliver better quality (critic/user scores) or stronger sales performance.

---

## 📌 Overview

Video game prices have increased over time, raising questions about whether higher prices reflect better quality or improved commercial success.

This project analyzes relationships between:

* Game pricing
* Critic scores
* User ratings
* Global sales

---

## ❓ Research Questions

1. How have video game prices changed over time?
2. Does price influence the relationship between critic and user scores?
3. Do higher-priced games generate more sales?

---

## 📊 Datasets

This project combines two datasets sourced from Kaggle:

### 1. Video Game Features & Pricing Dataset

* Source: Kaggle (Steam-based dataset)
* Original data collected from the Steam API
* Contains: pricing, release year, recommendations, and game metadata
* Size: ~16,720 rows, 16 columns

### 2. Video Game Sales & Ratings Dataset

* Source: Kaggle (aggregated from data.world)
* Contains: global sales, critic scores, and user scores
* Size: ~12,625 rows, 19 columns

### 🔑 Key Variables Used

* `PriceInitial` (game price)
* `Metacritic` (critic score)
* `User_Score` (user rating)
* `Global_Sales` (sales performance)
* `Year` (release year)

Each row in both datasets represents a single video game.

---

## 🧹 Data Preparation

* Merged datasets based on game title
* Removed duplicate entries
* Handled missing values
* Filtered relevant variables for analysis

---

## 📈 Methods

The analysis includes:

* Time series visualization (price trends over time)
* Correlation analysis (critic vs user scores)
* Linear regression models:

  * Price → Sales
  * Ratings → Sales
  * Interaction model (Price × Critic Score → User Score)

---

## 🔍 Key Findings

* 🎯 **Prices have increased over time**, especially after 2010
* ❌ **Price does NOT predict sales**
* ✅ **Critic scores are a significant predictor of sales**
* ❌ **User scores are not a strong predictor of sales**
* ❌ **Price does NOT change the relationship between critic and user scores**

---

## ⚠️ Limitations

* Sales data is highly skewed, which may affect regression assumptions
* Price data may not account for discounts or regional differences
* External factors (marketing, franchise popularity) are not included

---

## 🔮 Future Work

Future analysis could include:

* Genre or platform-specific trends
* Marketing or release timing effects
* More recent or expanded datasets

---

## 🛠️ Requirements

* pandas
* numpy
* matplotlib
* seaborn
* statsmodels

---

## ▶️ How to Run

1. Clone this repository
2. Place datasets in a `/data` folder
3. Open the notebook:

   ```
   video-game-price-analysis.ipynb
   ```
4. Run all cells

---

## 📁 Project Structure

```
├── data/
│   ├── vgsales.csv
│   ├── game_prices.csv
├── video-game-price-analysis.ipynb
└── README.md
```

---

## 💡 Summary

This project shows that while video game prices have increased over time, price alone is not a reliable indicator of quality or sales. Instead, critic reviews provide more meaningful insight into a game's success.
