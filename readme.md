# 🛒 Online Retail Customer Segmentation & Retention Analysis

A end-to-end data science project that analyses 373 days of UK online retail 
transactions to segment customers using RFM analysis and K-Means clustering, 
and recommends targeted retention strategies for each segment.

---

## Project Objective

- Understand customer purchasing behaviour from transaction-level data
- Engineer RFM (Recency, Frequency, Monetary) features per customer
- Segment customers using both rule-based scoring and K-Means clustering
- Validate clustering using Silhouette Score
- Provide data-driven retention strategies for each segment

---

## Dataset

- **Source**: [Online Retail Dataset — Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset)
- **Period**: December 2010 – December 2011 (373 days)
- **Records**: 397,884 transactions after cleaning
- **Region**: UK-based online retailer

---

## Results

### Rule-Based RFM Segments

| Segment | Customers | Revenue (£) | % of Total Revenue |
|---|---|---|---|
| Champions | 1,139 | £5,927,724 | 67.2% |
| Loyal Customers | 821 | £1,355,745 | 15.4% |
| At Risk | 643 | £800,532 | 9.1% |
| Lost | 1,065 | £519,409 | 5.9% |
| Needs Attention | 351 | £161,833 | 1.8% |
| Promising | 319 | £146,167 | 1.7% |

> **Champions represent 26.3% of customers but drive 66.5% of total revenue —
> protecting this segment is the highest business priority.**

### K-Means Clustering

- Optimal clusters: **k=4** (Silhouette Score: **0.6162**)
- Clusters identified: Champions, High Value, Loyal Customers, Lost
- K-Means results validated and consistent with rule-based segmentation

---

## 📁 Project Structure
```
Customer-Segmentation/
├── data/
│   ├── online_retail.csv               # Raw dataset (download from Kaggle)
│   ├── online_retail_cleaned.csv       # After cleaning
│   ├── rfm_data.csv                    # RFM scores + segments
│   └── rfm_clustered.csv              # RFM + K-Means clusters
├── 01_data_understanding.ipynb         # EDA & data cleaning
├── 02_rfm_feature_engineering.ipynb    # RFM calculation & scoring
├── 03_business_insights.ipynb          # Visualisations & recommendations
├── 04_kmeans_clustering.ipynb          # K-Means clustering & validation
├── requirements.txt
└── README.md
```
---

## 🚀 How to Run

1. Clone the repository
```bash
   git clone https://github.com/aryapatange/Customer-Segmentation.git
   cd Customer-Segmentation
```

2. Install dependencies
```bash
   pip install -r requirements.txt
```

3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset) and place it in the `data/` folder as `online_retail.csv`

4. Run notebooks in order — 01 → 02 → 03 → 04

---

## Retention Strategy Recommendations

| Segment | Strategy |
|---|---|
| Champions | Loyalty rewards, early product access, ask for reviews |
| Loyal Customers | Upsell higher-value products, referral programme |
| Promising | Welcome series, first repeat purchase discount |
| Needs Attention | Re-engagement email, personalised recommendations |
| At Risk | Win-back campaign, "We miss you" discount offer |
| Lost | Last-chance offer or deprioritise — low re-engagement ROI |

---

## Tech Stack

- **Python** — pandas, numpy, matplotlib, seaborn, scikit-learn
- **Jupyter Notebook**
- **Machine Learning** — K-Means clustering, StandardScaler
- **Analysis** — RFM feature engineering, Elbow Method, Silhouette Score

---

## 📈 Visualisations

<!-- Add a screenshot of your best visualisation here -->
<!-- Drag and drop an image into this section on GitHub -->

---

## 👤 Author

**Arya Patange**  
[GitHub](https://github.com/aryapatange)