# Cryptocurrencies

## Overview

Accountability Accounting is assessing cryptocurrencies for the possibility of providing clients an investment opportunity in a cryptocurrency portfolio. As part of this assessment visualizations will be created based upon the results of clustering the cryptocurrencies into different classes using unsupervised machine learning.

## Data Preprocessing

 - The data was cleaned, dropping cryptocurrencies that aren't being traded, currencies that don't have a working algorithm, and currencies where there have been coins mined.
 - Data types were altered so they could be used in scaling.
 - get_dummies() and StandardScaler() were used to scale the data for use with unsupervised ML.
 - Dimensions were reduced to 3 principal components

## Results

K-means was utilized to find the elbow curve to determine the appropriate number of clusters.

![K Means](Resources/images/elbow_curve.png)

PCS data was used to cluster the data in a 3d scatter plot using the number based from the elbow curve plot.

![3D Scatter](Resources/images/3d_scatter_with_clusters.png)

hvplot was used to create a scatter plot of the currencies based on Total Coin Supply and Total Coins Mined.

![Scatter Plot](Resources/images/scatter.png)
