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
Initialize each c in C with x picked from X

for i = 1 to t: do
  M <- b samples from X
  for x in M:
    d[x] <- f(C,x)  '''find the nearest centroid for each x
  end 
   
  for x in M:
    c <- d[x]   '''get cached ceter for x
    v[C] +=1    '''increase count of C by 1
    e = 1/v[C]   '''get per-center learning rate
    c = e * x + (1-e) * c
  end
end



Mini Batch K-means converges faster than K-means, but the quality is reduced.


# Documents
sk-learn documentation: 
http://scikit-learn.org/stable/modules/clustering.html#k-means

comparison:
https://algorithmicthoughts.wordpress.com/2013/07/26/machine-learning-mini-batch-k-means/
    



