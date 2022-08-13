# Cryptocurrencies

## Overview
### Purpose
The purpose of this project was to group a dataset of cryptocurrencies into clusters for classification using unsupervised machine learning. I first preprocessed the data, then used PCA to reduce the number of data dimensions. The data was then ready to be clustered using the K-means unsupervised learning algorithm. I used an elbow curve to find the optimal number of clusters, 4. Finally, I used Plotly Express and hvplot to visualize the clustered data.

## Results
I applied PCA to reduce the scaled dataset to three principal components, then used an elbow curve to find the best value for K, which I determined to be 4.
![image](https://user-images.githubusercontent.com/102445183/184458315-808f3245-c597-46fb-8385-8b17692b7f99.png)

I ran the K-means model with 4 clusters, which resulted in two larger clusters, one cluster with only 5 cryptocurrencies, and one cluster with only a single cryptocurrency. The cryptocurrency in it's own cluster was BitTorrent, with the most coins mined by far.
![image](https://user-images.githubusercontent.com/102445183/184458604-77580bc2-91d1-4b07-aaf3-561591c9730b.png)
![image](https://user-images.githubusercontent.com/102445183/184458679-fcd02fdf-c1ec-4529-ab56-6224e5ee68ea.png)

## Summary
### Recommendations
To improve the clustering, I would suggest removing the outlier BitTorrent data point. This change would allow for visualizations to be scaled to the rest of the data, and possibly new details being considered in the clustering.
