[1963] Anderson - Asymptotic theory for principal component analysis.md

This paper gives the asymptotic distributions of the characteristic roots and (normalized) vectors of a sample covariance matrix (where obs follow a multivariate normal and roots have an arbitrary multiplicity).

The linear combination with normalized weights of a random vector which maximizes the variance of the obtained random variable is the first principal component. 
The second principal component is the same as the first one (max. var.) except that it is independent (orthogonal) to the first principal component. 

The eigendecomposition of the covariance matrix gives orthonomal eigenvectors. 
When taking the dot product with the vectors of obs and the latter, we get the principal component.
(Note that when there is multiplicity greater than 1, there are some indeterminacy in the eigenvectors (linear comb. of the two eigenvectors also gives an eigenvector). Thus, in general, we choose eigenvectors that are orthogonals. 

The variance of the principal component (as a random variable obtained from the dotproduct between the random vector and the eigenvector of its cov. matrix) is equal to the eigenvalue of that eigenvector. 

They try to do inference of the eigenvalues/eigenvectors of a covariance matrix. In fine, they would like to identify non negligible sources of variance in the data. 
The model that have is given by a signal + error. And they assume the errors are uncorrelated and have equal variances. The overall sample is thus build from the variance in the true signal and the common error variance (which are considered small in comparison with signal variances). They test whether the smallest roots of the sample cov. matrix are all equal (and thus correspond to the error variances). 

The case where all roots of the correlation matrix are different are treated in Girshick 1939 (he gave the asymptoti variance and covariance, but not normality).
Lawley (1953) gave the variance and covariances of the smallest p-q roots being equal and different from the biggest roots. 
Barlett suggested the use of an approximate test distribution (chi-squared).

In this article authors assume normality of the data. 

**I did not understand the proofs and technicalities of this paper at all since it is not directly of the greatest importance if I am not determining the asymptotic distribution of my model.**
