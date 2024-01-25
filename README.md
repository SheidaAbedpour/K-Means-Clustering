
# K-Means Clustering

This repository contains two distinct projects that leverage the K-Means clustering algorithm for different applications. Each project is outlined below, providing an overview of the dataset, data preprocessing, and the custom K-Means implementation.

## K-Means Algorithm

K-Means is a popular clustering algorithm used in machine learning and data analysis. It is an unsupervised learning algorithm that partitions a dataset into K clusters, where each data point belongs to the cluster with the nearest mean. The primary objective of K-Means is to minimize the within-cluster variance, making data points within the same cluster as similar as possible.

Here's a more detailed explanation of how the K-Means algorithm works:

1.  **Initialization:**
   - Randomly select K data points from the dataset as the initial cluster centroids.
   - These centroids represent the initial guesses for the centers of the clusters.

2.  **Assignment:**
   - Assign each data point to the cluster whose centroid is the closest, typically using Euclidean distance.
   - The assignment is based on the distance between the data point and the centroid.

3.  **Update Centroids:**
   - Recalculate the centroids of the clusters by taking the mean of all data points assigned to each cluster.
   - The new centroids represent the updated cluster centers.

4.  **Repeat:**
   - Repeat the assignment and centroid update steps until convergence or a specified number of iterations.
   - Convergence occurs when the centroids no longer change significantly or when a certain number of iterations is reached.

### Key Concepts

- **Centroids:** The center points of the clusters. They are updated iteratively to better represent the center of the data points assigned to the cluster.

- **Cluster Assignment:** Determining which cluster each data point belongs to based on the distance to the centroids.

- **Within-Cluster Variance:** The measure of how spread out the data points are within each cluster. K-Means aims to minimize this variance.

### Considerations and Challenges:

- **Number of Clusters (K):** The number of clusters needs to be specified beforehand. Choosing the right K can be challenging and may require experimentation or domain knowledge.

- **Sensitivity to Initial Centroids:** K-Means can converge to different solutions based on the initial placement of centroids. Running the algorithm multiple times with different initializations is common.

- **Assumption of Spherical Clusters:** K-Means assumes that clusters are spherical and equally sized, which might not be suitable for all types of data.


### Use Cases:

- **Customer Segmentation:** Grouping customers based on purchasing behavior.
  
- **Image Compression:** Reducing the number of colors in an image by clustering similar pixel colors.

- **Anomaly Detection:** Identifying unusual patterns or outliers in a dataset.

- **Document Clustering:** Grouping similar documents together.


## Project 1: Image Segmentation using K-Means ✍️🔢

This project focuses on image segmentation using the K-Means clustering algorithm. 
The primary goal is to effectively segment and group handwritten digit images into clusters based on pixel intensity values. The project is particularly relevant in the context of digit recognition systems, where identifying distinct digit patterns is a crucial step.

### Results and Visualization
The script generates visualizations that showcase the clustering results. It typically includes:

- Clustered Digits: Images grouped into clusters based on similarities.
- Centroids: The final centroids representing the characteristic patterns within each cluster.

![Result](https://github.com/SheidaAbedpour/K-means/blob/main/handwritten-Digit-Recognition/handDigitClustring.png)

## Project 2: Customer Personality Analysis 🛍️🤔

In this project, K-Means clustering is applied to a marketing dataset. The dataset includes customer information, and the algorithm is utilized to identify patterns and group similar customers based on their features.

### Data Preprocessing
- ***One-Hot Encoding***: Categorical variables (Education, Marital_Status) are one-hot encoded and added to the dataframe.
- ***Date Transformation***: The Dt_Customer column is converted to datetime and transformed to represent the number of days since the customer joined.
- ***Standard Scaling***: The data is standardized using the StandardScaler from scikit-learn.

![Result](https://github.com/SheidaAbedpour/K-Means-Clustering/blob/main/Customer-Personality-Analysis/result.PNG)

## Conclusion
These projects demonstrate the versatility of the K-Means clustering algorithm in different domains—image segmentation and customer segmentation within a marketing dataset. Users can explore the provided code, customize parameters, and adapt it to their specific needs.

## Lecture
- University: Isfahan University - Faculty of Computer Engineering
- Course: Linear Algebra
- Student Name: Sheida Abedpour
- Date: December 2023

