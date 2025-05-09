# Customer Segmentation using K-Means

This project applies **unsupervised machine learning** techniques, specifically **K-Means clustering**, to segment credit card customers into distinct behavioral groups based on their spending patterns and financial activity.

---

##  Dataset

- **Source**: Kaggle – [Credit Card Customer Segmentation Dataset](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)
- **Key Features Used**:
  - `BALANCE`
  - `PURCHASES`
  - `CASH_ADVANCE`
  - `CREDIT_LIMIT`
  - `PAYMENTS`
  - `MINIMUM_PAYMENTS`

---

##  Project Pipeline

### 1. **Data Cleaning and Imputation**
- Handled missing values using median imputation.
- Converted data types where necessary for numeric processing.

### 2. **Outlier Handling**
- Applied **Winsorizing** (IQR method with 1.5 * IQR cap) to reduce the impact of outliers while preserving data size.

### 3. **Feature Scaling**
- Used `StandardScaler` to normalize features before clustering.

### 4. **Optimal Number of Clusters**
- **Elbow Method**: Identified K=3 as a good trade-off between inertia and overfitting.
- **Silhouette Score**: Achieved a score of **0.224**, indicating moderate but meaningful cluster separation.

### 5. **K-Means Clustering**
- Applied `KMeans(n_clusters=3)` on the scaled data.
- Assigned each customer to one of three distinct clusters.

### 6. **Dimensionality Reduction (PCA)**
- Reduced to 2D using **Principal Component Analysis** for visualization purposes.

### 7. **Cluster Interpretation**
- **Cluster 0 – Engaged Transactors**: High spenders, responsible users with high usage and low debt.
- **Cluster 1 – High Spenders**: Frequent, large-scale spenders with higher credit limits.
- **Cluster 2 – Low Spenders**: Low activity, low credit usage, often below average spending.

---

## 📊 Visualizations

-  **Elbow Method Plot** – to determine optimal `K`
-  **Silhouette Score Plot** – for cluster quality evaluation
- **PCA Scatter Plot** – 2D visualization of clusters
-  **Cluster Feature Means (Bar Charts)** – highlight differences in behavior between segments

---

## ✅ Results Summary

- **K-Means Clusters**: 3 optimal clusters
- **Silhouette Score**: `0.224`
- **Insights**:
  - Clear segmentation between high-value and low-value customers
  - High-value groups (Cluster 0 and 1) show potential for loyalty programs
  - Low-spenders (Cluster 2) offer room for up-selling or targeted promotions

---

## 💡Business Recommendations

| Segment              | Strategy                                                                 |
|----------------------|--------------------------------------------------------------------------|
| **Engaged Transactors** | Promote **rewards programs**, premium credit offers, loyalty bonuses         |
| **High Spenders**        | Offer **exclusive benefits**, travel perks, and VIP support               |
| **Low Spenders**         | Use **targeted marketing**, increase credit education, offer incentives  |

---

## Tech Stack

- **Python**, `pandas`, `numpy`
- **Scikit-learn** – for clustering, scaling, and PCA
- **Matplotlib** / **Seaborn** – for visualizations

---

##  How to Run

1. Clone the repository  
2. Install requirements: `pip install -r requirements.txt`  
3. Run the notebook: `Customer_Segmentation_KMeans.ipynb`  
4. Follow the analysis step-by-step
"""


