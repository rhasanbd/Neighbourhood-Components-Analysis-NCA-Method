# Neighbourhood Components Analysis (NCA) Method

In this notebook, we present the Neighbourhood Components Analysis (NCA) method for learning a Mahalanobis distance measure to be used in the the K Nearest Neighbors (K-NN) classification. 
https://cs.nyu.edu/~roweis/papers/ncanips.pdf

The NCA addresses two key limitations of K-NN:

- Computational: K-NN needs to store the entire training dataset and compute distance with all training points
- The absence of an optimal distance metric in K-NN


The NCA method addresses the above two limitations by "learning" a distance metric for a given problem. 

- NCA finds a linear transformation of input data such that the average leave-one-out (LOO) classification performance is maximized in the transformed space. 

- The learned distance metric of NCA is low rank, thus substantially reduces storage and search costs at test time.


The learned Mahalanobis distance measure of NCA is used by a K-NN classifier model. 


## Task

We compare the performance of the K-NN on the transformed feature space of NCA and the original feature space.  
