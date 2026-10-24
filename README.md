# Strategic Customer Segmentation for E-commerce Growth
**Framework:** CRISP-DM | **Methodology:** RFM Modeling & K-Means Clustering

## 📌 Project Overview
This project focuses on identifying high-value customer segments for a Brazilian E-commerce platform (Olist) using a data-driven approach. By analyzing transaction history, I developed a segmentation model to help Marketing and FP&A teams optimize customer retention strategies and improve revenue forecasting.

## 🛠️ Tech Stack & Methodology
* **Environment:** Python (Google Colab)
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (StandardScaler, KMeans)
* **Visualization:** Plotly (3D Interactive), Matplotlib, Seaborn
* **Framework:** Followed the **CRISP-DM** lifecycle (Business Understanding → Data Prep → Modeling → Evaluation).

## 📊 Key Analytical Steps

### 1. Feature Engineering (RFM)
I aggregated over 100k records to create three core metrics for each unique customer:
* **Recency ($R$):** Days since the last purchase.
* **Frequency ($F$):** Total number of distinct orders.
* **Monetary ($M$):** Total revenue generated per customer.

### 2. Finding the Optimal Clusters
Using the **Elbow Method**, I identified $k=3$ as the optimal number of clusters where the Within-Cluster Sum of Squares (Inertia) began to level off.

![Elbow Method](RFM_Elbow%20method.png)

### 3. Machine Learning Model
To ensure accuracy, I applied **Log Transformation** to handle skewed data and **Standard Scaling** before fitting the K-Means algorithm.

## 📈 Strategic Insights
The model identified three distinct customer personas:

* 🏆 **Champions:** High frequency and high spenders. They are the backbone of predictable revenue.
* 🌱 **Potential:** Recent buyers who have only purchased once. They represent the primary target for cross-selling.
* ❄️ **Hibernating:** Long-lost customers. Analysis suggests a "sunset" strategy to optimize marketing spend.

![3D RFM Clusters](RFM%203D%20Clusters.png)

## 🚀 Business Impact & Recommendations
* **For FP&A:** Use "Champion" segment behavior to set more accurate baseline revenue targets.
* **For Marketing:** Implement a loyalty program for "Champions" and a personalized "Next-Best-Offer" campaign for the "Potential" segment.
* **Operational Efficiency:** Reallocate budget away from "Hibernating" segments to improve overall ROI.

---
*Developed as part of my career transition into Business Analytics and Financial Planning & Analysis (FP&A).*
