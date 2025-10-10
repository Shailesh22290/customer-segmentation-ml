
# Customer Segmentation for Targeted Marketing

This project applies **unsupervised machine learning** to identify distinct customer groups based on their purchasing behavior and demographics.  
The goal is to help businesses design **personalized marketing strategies** and optimize resource allocation.

---

## 📊 Project Overview

**Objective:**  
To segment customers into meaningful clusters using behavioral and transactional data, enabling data-driven marketing insights.

**Techniques Used:**
- RFM (Recency, Frequency, Monetary) feature engineering
- Clustering algorithms: K-Means, DBSCAN
- PCA/UMAP for dimensionality reduction and visualization
- Power BI dashboard for cluster insights

---

## 🧱 Project Pipeline

1. **Data Collection**
   - Public datasets used:
     - [Mall Customers (Kaggle)](https://www.kaggle.com/datasets/shwetabh123/mall-customers)
     - [Online Retail (UCI)](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
   - Place your dataset in the `data/` folder.

2. **Data Preprocessing**
   - Handle missing values and duplicates
   - Feature scaling and normalization
   - Extract RFM metrics (Recency, Frequency, Monetary value)

3. **Exploratory Data Analysis (EDA)**
   - Distribution plots and pairplots for key features
   - Correlation analysis
   - Outlier detection

4. **Feature Engineering**
   - RFM calculation (for transactional datasets)
   - Categorical encoding and normalization

5. **Clustering**
   - K-Means with elbow and silhouette analysis
   - DBSCAN for density-based clustering
   - Evaluate cluster stability and interpret results using SHAP-like importance measures (optional)

6. **Visualization**
   - PCA and UMAP projections for 2D cluster visualization
   - Power BI dashboard for real-time business interpretation

7. **Insights & Action Plan**
   - Identify high-value, loyal, at-risk, and churned customer segments
   - Propose targeted campaigns and retention strategies

---

## 🧰 Tech Stack

| Category | Tools & Libraries |
|-----------|------------------|
| **Language** | Python |
| **Data Handling** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn, Plotly |
| **ML / Clustering** | Scikit-learn, DBSCAN, KMeans |
| **Dimensionality Reduction** | PCA, UMAP |
| **Dashboard** | Power BI |
| **Export** | Joblib (model), CSV (for BI) |

---

## 🚀 How to Run

1. Clone this repository  
   ```bash
   git clone https://github.com/<your-username>/customer-segmentation.git
   cd customer-segmentation


2. Create and activate a Conda environment

   ```bash
   conda create -n segmentation python=3.10 -y
   conda activate segmentation
   ```

3. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

4. Place dataset (e.g., `Online Retail.xlsx`) inside the `data/` folder

5. Run the notebook or script

   ```bash
   jupyter notebook "Customer Segmentation — Notebook (RFM + Clustering).ipynb"
   ```

6. Export cluster-labeled data to CSV for Power BI visualization

---

## 📈 Deliverables

* **Python Notebook:** Full clustering pipeline (`Customer Segmentation — Notebook (RFM + Clustering).ipynb`)
* **Exported CSV:** Cluster assignments for each customer
* **Power BI Dashboard:** Interactive cluster insights
* **Business Report:** Key findings and marketing strategies

---

## 📂 Folder Structure

```
customer-segmentation/
│
├── data/
│   └── Online Retail.xlsx
│
├── notebooks/
│   └── Customer Segmentation — Notebook (RFM + Clustering).ipynb
│
├── outputs/
│   ├── cluster_visualizations/
│   └── segmented_customers.csv
│
├── requirements.txt
└── README.md
```

---

## 📚 References

* [Kaggle – Mall Customers Dataset](https://www.kaggle.com/datasets/shwetabh123/mall-customers)
* [UCI Machine Learning Repository – Online Retail](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
* “RFM Segmentation for Customer Analytics” – Towards Data Science

---

## 🧩 Future Improvements

* Deploy automated pipeline (Airflow / Docker)
* Integrate with CRM or marketing automation APIs
* Experiment with deep clustering and self-organizing maps (SOMs)
* Add a web dashboard using Streamlit or Plotly Dash

---

### 👨‍💻 Author

**Shailesh Kachhi**
[LinkedIn](https://linkedin.com/in/shailesh-kachhi) | [GitHub](https://github.com/your-username)



