# Customer Clustering using Unsupervised Machine Learning

## Overview

This project aims to cluster customers of an automobile company to help the marketing team better understand the target audience for their products. By identifying groups of similar customers, the marketing team can design more targeted and effective campaigns.

## Methodology

1. **Data Cleaning & Exploration**: We began by cleaning the dataset, handling missing values, and exploring the features to gain a better understanding of the data.
2. **Data Preprocessing**: We preprocessed the data by encoding categorical variables and scaling numerical variables to ensure that all features contribute equally to the clustering process.
3. **Unsupervised Machine Learning Models**: We applied various unsupervised machine learning models, including KMeans, DBSCAN, Agglomerative Clustering, and Gaussian Mixture Model, to identify customer segments.  The dataset was preprocessed to handle missing values and scaled to ensure better performance of the algorithms.
4. **Model Evaluation**: We evaluated the performance of each model using Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index to determine the most suitable model for our purpose.
5. **Model Selection**: Based on the evaluation metrics, we chose the best-performing model for our customer segmentation task.


### Evaluation Metrics

We used three evaluation metrics to assess the performance of these algorithms:

1. **Silhouette Score**: Ranges from -1 to 1. A higher score indicates that the clusters are well-separated and the data points within a cluster are similar to each other.
2. **Calinski-Harabasz Index**: Evaluates the ratio of between-cluster variance to within-cluster variance. A higher score indicates better clustering performance.
3. **Davies-Bouldin Index**: Measures the average similarity between clusters. A lower score indicates better clustering performance, as it means the clusters are less similar to each other.

## Results

DBSCAN has the highest Silhouette Score (0.1588) and the lowest Davies-Bouldin Index (1.5468), suggesting that it creates well-separated and dissimilar clusters. Although KMeans has a better Calinski-Harabasz Index, indicating better separation of cluster variance, the overall performance of DBSCAN is more consistent across the evaluation metrics.

## Conclusion

For this project, we can consider DBSCAN as the best choice for clustering the customer data. It provides the most consistent performance across the evaluation metrics and helps in creating well-separated and dissimilar clusters. This information will be valuable for the marketing team in designing targeted and effective campaigns for different customer segments.

