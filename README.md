# Customer Segmentation using KMeans

This project applies unsupervised learning (KMeans clustering) to segment credit card customers into behavioral groups based on spending patterns and financial activity.

## Dataset
- Source: [Kaggle - Credit Card Customer Segmentation](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)
- Contains features such as balance, purchases, cash advance, credit limit, and payments.

##  Project Steps

1. Data Cleaning and Imputation
2. Feature Engineering (Ratios)
3. Normalization (StandardScaler)
4. Clustering with KMeans (K=2)
5. PCA for visualization
6. Cluster interpretation and business recommendations

## Visualizations

- PCA Scatter Plot
- Cluster Feature Means (Bar Chart)
- Heatmap of Feature Differences

## Files

- `Customer_Segmentation.ipynb`: Full code
- `Report.pdf`: Detailed analysis and insights
- `plots/`: Contains all result images
- `dataset/`: Original dataset used

## Results

- 2 clusters discovered with a Silhouette Score of **0.279**
- Clear separation between high-value and risk-prone customers
- Strategic business actions proposed for both segments

