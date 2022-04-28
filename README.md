# Cryptocurrencies

## Overview:

The goal of this study was to use CryptoCompare data to provide a report and visualisation of currently traded cryptocurrencies that might be put together to form a new classification system. This report will be utilised to assist *Accountability Accounting* in providing its customers with a new investment portfolio in the fascinating world of cryptocurrencies.

We needed to preprocess the data to construct an unsupervised Machine Learning model that would allow us to run a clustering algorithm to group the cryptocurrencies because the data had no known outcome.

We learned and applied the following during this investigation:

* `Data Preprocessing (Selection, Transformation, and Scaling)` is a technique for preparing data for Machine Learning Algorithms.
* `Elbow Curve` - a method for determining the optimal number of clusters for an algorithm to categorise items by.
* `Principal Component Analysis (PCA)` is a statistical technique which is used when the number of features in a machine learning method is too large,  technique for speeding up the algorithm.
* `Clustering Algorithms (KMeans)` is the process of forming clusters out of comparable objects or data points.
* `Visualization (hvPlot, Plotly)` are graphic libraries that enable us to generate 2D and 3D graphics vizualization.

## Results:

Only 1,144 cryptocurrencies were currently trading in the initial dataset, which included 1,252 items. Null values were removed from the data, leaving only cryptocurrencies with a total number of produced coins greater than 0. In the end, 532 marketable cryptocurrencies were discovered.

![Image1](../Images/Image1.png)

The *Elbow Curve* method showed the slope at 4. This is the number of clusters that was used for the `KMeans` algorithm.

![Image2](../Images/Image2.png)

The clusters are plotted in a 3D scatter plot for visualization.

![Image3](../Images/Image3.png)

## Resources Used:
* Dataset from [CryptoCompare](../Resources/cryto_data.csv)
* Software: Python 3.7.11 (mlenv), VSCode 1.66.2
* Libraries: Scikit-learn, Plotly, hvPlot, Pandas