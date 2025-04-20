# 🎮 Video Game Sales: Insights & Prediction

A data analysis and regression-based prediction project exploring regional video game sales across platforms, genres, and publishers. Combines SQL querying, detailed visualization, and machine learning models to uncover market trends and forecast sales.

---

## 📁 Dataset

- **Source:** [Kaggle - Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogame-sales-with-ratings)
- **Fields:** Name, Platform, Year, Genre, Publisher, Sales (NA/EU/JP/Other/Global)

---

## 🛠️ Tools & Tech

- **Languages:** Python, SQL  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, LightGBM  
- **Database:** MySQL Workbench 8.0 CE  
- **Environments:** Google Colab, MySQL  

---

## 🧮 Key Objectives

- Analyze regional and platform-based trends in video game sales.  
- Identify dominant publishers and genre preferences by region.  
- Explore evolution of platforms and title releases over time.  
- Forecast global sales using regression models.  

---

## 📊 Analytical Insights

### 🔹 Publisher Analysis  
- Identified top publishers by region and genre.  
- Used grouped bar charts and heatmaps to highlight specialization trends.  

### 🔹 Sales Distribution  
- Plotted histograms and boxplots to analyze skewed sales data.  
- Applied log transformation for normalization and clarity.  

### 🔹 Top Games Analysis  
- Ranked best-selling titles across platforms and years.  
- Explored contributing factors like platform, release year, and genre.  

### 🔹 Platform Evolution  
- Tracked sales trends of major consoles over time.  
- Highlighted impactful platform launches using time series plots.  

### 🔹 Year-wise Breakdown  
- Analyzed annual game releases and sales patterns.  
- Dual-axis plots used to correlate game count with global sales.  

---

## 🤖 Predictive Modeling

- **Models Used:** Linear Regression, Decision Tree, Random Forest, Gradient Boosting, SVR, XGBoost, LightGBM  
- **Evaluation Metrics:** MAE, MSE, R² Score  
- **Best Model:** Linear Regression (R² = 0.96)

> Models trained on scaled features to forecast Global_Sales; evaluated on test set performance.

---

## 🧾 SQL Highlights

- Loaded dataset into MySQL and executed regional/platform aggregations.  
- Example query:
```sql
SELECT Platform, SUM(NA_Sales) AS Total_NA_Sales
FROM vg_sales
GROUP BY Platform
ORDER BY Total_NA_Sales DESC;
```
---

## 📄 License
This project is licensed under the Apache License 2.0. See the LICENSE file for details.
