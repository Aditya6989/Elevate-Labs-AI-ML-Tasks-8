1. How does K-Means clustering work?
K-Means clustering is an unsupervised learning algorithm used to group data into clusters. Here’s how it works:
Initialization: Select 
𝐾
K random points as cluster centroids.
Assignment: Assign each data point to the nearest centroid.
Update: Calculate the new centroid as the mean of all points in a cluster.
Repeat: Keep assigning and updating until centroids no longer change significantly.
Think of it as grouping similar data points based on their proximity to the "center" of each group.

2. What is the Elbow method?
The Elbow method helps find the optimal number of clusters (
𝐾
K) by calculating the WCSS (Within-Cluster Sum of Squares) for different values of 
𝐾
K.
Plot WCSS against 
𝐾
K.
The point where the WCSS reduction slows down significantly (forming an "elbow") is considered the optimal number of clusters.
This method helps balance model complexity and performance, avoiding both underfitting and overfitting.

3. What are the limitations of K-Means?
Fixed Number of Clusters: You need to specify 
𝐾
K beforehand, which can be tricky.
Sensitive to Outliers: Outliers can disproportionately affect centroid calculation.
Spherical Clusters: Works best when clusters are roughly spherical and similar in size.
Random Initialization: Different starting points can lead to different results.
Not Suitable for Complex Shapes: Struggles with clusters that are non-convex or irregularly shaped.

4. How does initialization affect results?
K-Means can end up in a local minimum due to random centroid initialization. This means the clusters might not be optimal.
To address this, the algorithm usually runs several times with different initializations (like K-Means++) and picks the best result.
If initialization is poor, the algorithm might converge to suboptimal clusters.

5. What is inertia in K-Means?
Inertia measures how tightly the data points are clustered around centroids.
Mathematically, it is the sum of squared distances between each point and its assigned centroid.
Lower inertia indicates more compact clusters.
Inertia is used as a metric to evaluate how well the model has clustered the data.

6. What is Silhouette Score?
The Silhouette Score measures how similar an object is to its own cluster compared to other clusters.
Range: -1 to 1
High value (close to 1): Points are well matched within their cluster.
Low value (close to -1): Points may have been assigned to the wrong cluster.
A higher Silhouette Score indicates better-defined clusters.

7. How do you choose the right number of clusters?
Elbow Method: Find the point where adding more clusters doesn't significantly reduce WCSS.
Silhouette Score: Check which number of clusters has the highest average score.
Domain Knowledge: Sometimes, you may have prior knowledge of how many clusters to expect.
Gap Statistic: Compares the WCSS of the clustering to a null reference distribution.
Often, a combination of these methods gives a more reliable choice.

8. What’s the difference between clustering and classification?
Clustering: Unsupervised learning where data is grouped based on similarities without predefined labels.
Classification: Supervised learning where the algorithm learns from labeled data to predict categories.
In short, clustering finds hidden patterns, while classification predicts predefined categories