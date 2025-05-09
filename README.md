Customer Segmentation using KMeans

This project applies unsupervised learning (K-Means clustering) to segment credit card customers into behavioral groups based on their spending patterns and financial activity.

Dataset
Source: Kaggle - Credit Card Customer Segmentation

Contains features such as balance, purchases, cash advance, credit limit, and payments.

Project Steps
Data Cleaning and Imputation

Outlier Handling (Winsorizing)

Feature Scaling (StandardScaler)

Determining Optimal Clusters (Elbow Method, Silhouette Score)

Clustering with KMeans (K=3)

PCA for visualization

Cluster interpretation and business recommendations

Visualizations
Elbow Method Plot

Silhouette Score Plot

PCA Scatter Plot

Cluster Feature Means (Bar Charts)

Results
3 clusters discovered using K-Means, with an optimal number of clusters determined by both the Elbow Method and Silhouette Score.

The Silhouette Score for the K-Means clustering is 0.224.

Identified distinct customer segments:

Engaged Transactors (Cluster 0): High spending activity, frequent card usage, and responsible credit behavior.

High Spenders (Cluster 1): High spending activity, frequent card usage and responsible credit behavior.

Low Spenders (Cluster 2): Lower spending and credit limits, moderate card usage.

Strategic business actions are proposed for each segment, focusing on retention for high-value customers and growth for lower-activity segments.
