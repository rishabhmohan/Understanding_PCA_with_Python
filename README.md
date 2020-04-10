PCA is a dimensionality reduction technique, and is used in high dimensionality data to find patterns. 
An excellent resource to understand PCA, eigenvector, eigenvalues: https://pathmind.com/wiki/eigenvector 

### Steps in PCA:
1. Get data X (n*p dimension)
2. Get covariance matrix (p*p dimension)
3. Do eigendecomposition that would give pair of eigenvalues (p dimension vector) and eigenvectors (p*p dimension vector)
4. We can sort eigenpairs by descending order of eigenvalues
5. Collect the two eigenvectors (or more) that correspond to the two largest eigenvalues, to capture about most of the variance in this dataset. Get more eigenvectors to capture more variance.
6. This would create a n*2-dimensional projection matrix W from the top two eigenvectors.
7. Using the projection matrix, we can now transform entire training dataset onto the PCA subspace (the principal components one and two) obtaining x′, now a two-dimensional sample vector consisting of two new features by calculating dot product of projection matrix W and dataset X. This transformed dataset would be n*2 dimensional dataset.
