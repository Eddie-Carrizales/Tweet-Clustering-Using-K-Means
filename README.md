# Tweets Clustering Using K-Means

In this project I implemented Tweets clustering using K-means (and Jaccard Distance).

After implementation I ran multiple trials for different values of K (i.e, number of clusters), and plotted the results to create an elbow method graph.

More details on the trials and a picture of the elbow method graph can be seen in the other files.

# Further Project Explanations:

# Jaccard Distance:
The Jaccard distance measures dissimilarity between two sample sets (A and B). It is defined as the difference of the sizes of the union and the intersection of two sets divided by the size of the union of the sets.

A tweet can be considered as an unordered set of words such as {a,b,c}. By "unordered", we mean that {a,b,c}={b,a,c}={a,c,b}= etc.

A Jaccard Distance Dist(A, B) betwee tweet A and B has the following properties:
  * It is small if tweet A and B are similar.
  * It is large if they are not similar.
  * It is 0 if they are the same.
  * It is 1 if they are completely different (i.e., no overlapping words).

# K - means:
K-means is a classic unsupervised data clustering algorithm. 

K-means uses k centroids (points which are the center of a cluster) to define clusters. A data point is considered to be in a particular cluster if it is closer to that cluster's centroid than any other centroid. The main steps of K-means are as follows: 
  1. Define k centroids, one for each cluster. The algorithm usually chooses the initial centroids randomly from the data set. 
  2. The K-means algorithm iterates between the following two steps until it converges:
      * Assign data points to clusters based on the current selection of the centroids.
      * Compute the new centroids based on the updated assignment of data points to clusters.

Note: The algorithm is considered to converge when the assignment of data points to clusters no longer changes.
