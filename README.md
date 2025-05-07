# K-Means Clustering

## Overview

This project demonstrates clustering using the K-Means algorithm in Python. The script loads a dataset, applies K-Means clustering, visualizes the clusters, and evaluates the clustering quality using the Elbow method and Silhouette Score.

## Features

* Loads and preprocesses the data.
* Uses the Elbow method to determine the optimal number of clusters.
* Fits the K-Means model and assigns cluster labels.
* Visualizes clusters using PCA (if dimensionality > 2).
* Evaluates clustering performance with the Silhouette Score.

## Requirements

* Python 3.x
* pandas
* numpy
* matplotlib
* scikit-learn

## Installation

To install the required packages, run:

```
pip install pandas numpy matplotlib scikit-learn
```

## Usage

1. Place your dataset file (CSV format) in the same directory.
2. Run the script:

```
python k_means_clustering.py
```

## Output

* Cluster visualization with centroids.
* Optimal number of clusters (using the Elbow method).
* Silhouette Score for evaluating clustering quality.

## Notes

* The dataset should have numeric features.
* The Elbow method plot will guide you in selecting the optimal number of clusters.
