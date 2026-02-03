# 📊 Trader Behavior & Market Sentiment Analysis

## 📌 Project Overview

This project analyzes the relationship between **Bitcoin Market Sentiment (Fear & Greed Index)** and **Historical Trader Performance (Hyperliquid Data)**.

The main objective is to understand how different market sentiment regimes (such as Fear, Greed, and Extreme Greed) influence:

- Trader profitability  
- Trading activity  
- Risk-taking behavior  
- Performance across different trader segments (Retail, High-volume, Whale)

The analysis goes beyond basic data cleaning and focuses on uncovering meaningful behavioral patterns and actionable insights.

---

## 📂 Datasets Used

### 1. Bitcoin Market Sentiment Dataset
**Columns include:**
- `timestamp`
- `value` (Fear & Greed Index score)
- `classification` (Fear, Greed, Neutral, etc.)
- `date`

### 2. Historical Trader Data (Hyperliquid)
**Columns include:**
- `Account`
- `Coin`
- `Execution Price`
- `Size USD`
- `Side`
- `Timestamp`
- `Closed PnL`
- `Fee`
- and others

---

## 🛠️ Tools & Technologies

- **Python 3.9+**
- **Google Colab / Jupyter Notebook**
- **Libraries:**
  - pandas
  - numpy
  - matplotlib
  - seaborn

---

## 🔄 Project Workflow

### ✅ Step 1: Data Ingestion & Cleaning
- Loaded both datasets
- Converted timestamps to daily format
- Handled missing values

### ✅ Step 2: Time-Series Alignment
- Merged trader data with sentiment data using daily dates

### ✅ Step 3: Feature Engineering
Calculated key performance metrics:

- Win Rate
- Average Trade Size
- Total Trading Volume
- Total Closed PnL
- Average Closed PnL

### ✅ Step 4: Trader Segmentation
Traders were grouped into:

- Retail  
- High-volume  
- Whale  

Based on total trading volume.

### ✅ Step 5: Exploratory Data Analysis (EDA)

Visualizations included:

- Bar charts by sentiment category  
- Grouped bar charts by sentiment and trader segment  
- Boxplots of profit distribution  
- Correlation matrix and heatmap  

### ✅ Step 6: Correlation Analysis
Explored relationships between:

- Sentiment score  
- Daily profitability  
- Trading volume  

---

## 📈 Key Insights

- Fear and Extreme Greed periods showed the highest trading activity and profitability  
- Whale traders consistently generated the highest total profits  
- Retail traders performed best during Neutral and Extreme Greed periods  
- High-volume traders struggled most during Extreme Fear conditions  
- Trading volume was strongly linked to total profitability  

---

## ✅ Actionable Recommendations

- Traders should adapt strategies based on sentiment conditions  
- Strong risk management is crucial during Fear-driven markets  
- Retail traders can focus more on Neutral and Extreme Greed periods  
- High-volume traders should improve strategies during Extreme Fear  
- Whale traders can continue leveraging volatility strategically  

---

## 📁 Files Included

- `Trade_behavior_sentiment_analysis.ipynb` → Complete analysis notebook  
- `README.md` → Project documentation  

---

## ▶️ How to Run the Project

### Option 1: Google Colab (Recommended)

1. Open https://colab.research.google.com  
2. Upload `notebook.ipynb`  
3. Click **Runtime → Run all**

### Option 2: Jupyter Notebook (Local)

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook
