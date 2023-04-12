# Customer Segmentation Project
This project aims to help an automobile company entering new markets by segmenting potential customers into groups based on their similarities. By understanding these segments, the company can create targeted marketing strategies for each group, ultimately increasing sales and customer satisfaction.

Overview
We used a dataset containing information about potential customers, including their demographics, spending habits, and preferences. Our goal was to identify clusters of similar customers to assist the company in their marketing efforts.

Methodology
Data Cleaning & Exploration: We began by cleaning the dataset, handling missing values, and exploring the features to gain a better understanding of the data.

Data Preprocessing: We preprocessed the data by encoding categorical variables and scaling numerical variables to ensure that all features contribute equally to the clustering process.

Unsupervised Machine Learning Models: We applied various unsupervised machine learning models, including KMeans, DBSCAN, Agglomerative Clustering, and Gaussian Mixture Model, to identify customer segments.

Model Evaluation: We evaluated the performance of each model using Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index to determine the most suitable model for our purpose.

Model Selection: Based on the evaluation metrics, we chose the best-performing model for our customer segmentation task.

Results
We have applied four different unsupervised machine learning algorithms (KMeans, DBSCAN, Agglomerative Clustering, and Gaussian Mixture Model) to group similar customers. We have used three evaluation metrics to assess the performance of these algorithms:

Silhouette Score: This score ranges from -1 to 1. A higher score indicates that the clusters are well-separated and the data points within a cluster are similar to each other. In our results, DBSCAN has the highest Silhouette Score (0.1588), which means it performed better than the other algorithms in creating well-separated and cohesive clusters.

Calinski-Harabasz Index: This index evaluates the ratio of between-cluster variance to within-cluster variance. A higher score indicates better clustering performance. In our results, KMeans has the highest Calinski-Harabasz Index (249.1751), which means it performed better than the other algorithms in creating clusters with larger between-cluster variance compared to within-cluster variance.

Davies-Bouldin Index: This index measures the average similarity between clusters. A lower score indicates better clustering performance, as it means the clusters are less similar to each other. In our results, DBSCAN has the lowest Davies-Bouldin Index (1.5468), which means it performed better than the other algorithms in creating dissimilar clusters.                                                                               
                                                                                                                                                                In summary, considering the evaluation metrics, DBSCAN seems to be the best choice for this dataset. It has the highest Silhouette Score (0.1588) and the lowest Davies-Bouldin Index (1.5468), suggesting that it creates well-separated and dissimilar clusters. Although KMeans has a better Calinski-Harabasz Index, indicating better separation of cluster variance, the overall performance of DBSCAN is more consistent across the evaluation metrics. Therefore, for this project, we can consider DBSCAN as the winner and the preferred algorithm for clustering the customer data.
The selected model successfully segmented the potential customers into distinct groups, enabling the company to develop targeted marketing strategies for each segment. By understanding the characteristics of these customer groups, the company can tailor their marketing efforts to appeal to the unique needs and preferences of each segment, ultimately improving sales and customer satisfaction.
