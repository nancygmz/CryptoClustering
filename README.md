# Cryptocurrency Clustering Project

## Introduction

This repository contains a Python project that uses unsupervised learning techniques, specifically K-means clustering, to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. The project involves data preprocessing, dimensionality reduction using Principal Component Analysis (PCA), and clustering analysis.

## Key Steps and Findings

### Data Preprocessing

- Renamed the notebook file to `Crypto_Clustering.ipynb`.
- Loaded the cryptocurrency market data from `crypto_market_data.csv` into a DataFrame.
- Conducted exploratory data analysis, including summary statistics and data visualization, to understand the dataset.

### Scaling Data

- Normalized the data using the `StandardScaler()` module from scikit-learn.
- Created a new DataFrame with the scaled data while preserving the "coin_id" index.

![image](https://github.com/nancygmz/CryptoClustering/blob/main/images/scaled_data.png)

### Finding the Best Value for k

- Utilized the elbow method to determine the optimal value for k (number of clusters) using the original scaled data.
- Found the best value for k based on the elbow method.

![image](https://github.com/nancygmz/CryptoClustering/blob/main/images/best_k_value.png)

### Clustering Cryptocurrencies with K-means

- Clustered cryptocurrencies using the best value for k on the original scaled data.
- Visualized the clusters using a scatter plot and labeled points with cryptocurrency names.

![image](https://github.com/nancygmz/CryptoClustering/blob/main/images/clustering%20with%20k%20means.png)

### Principal Component Analysis (PCA)

- Performed PCA on the original scaled data to reduce features to three principal components.
- Calculated the explained variance to assess the significance of each component.

### Finding the Best Value for k with PCA

- Applied the elbow method to determine the best value for k using the PCA-transformed data.
- Compared the best k value found with PCA to the best k value found with the original data.

![image](https://github.com/nancygmz/CryptoClustering/blob/main/images/PCA_elbow.png)

### Clustering with PCA Data

- Clustered cryptocurrencies using the best value for k on the PCA-transformed data.
- Visualized the clusters using a scatter plot with cryptocurrency names.

![image](https://github.com/nancygmz/CryptoClustering/blob/main/images/PCA_cluster.png)

## Conclusion

This project demonstrates the use of unsupervised learning techniques to cluster cryptocurrencies based on price changes. It explores the impact of dimensionality reduction through PCA on clustering results. By following the steps outlined in the notebook, you can gain insights into how different approaches affect the clustering of cryptocurrency data.
