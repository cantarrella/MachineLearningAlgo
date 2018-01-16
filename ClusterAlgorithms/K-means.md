# K-means v.s. Mini Batch K-means

## K-means

Given paramters
k: number of clusters

Algorithm: EM algorithm.



## Mini Batch K-means

Ideas, in each iteration, randomly sample a batch of data of size b, then update the centroids accordingly.

Input: k, b, t, X
k: number of clusters C
b: batch size
t: number of iterations
X: dataset


Algorithm:
Initialize each $c \in C$ with $x$ picked from $X$

$ \sum_{\forall i}{x_i^{2}} $



