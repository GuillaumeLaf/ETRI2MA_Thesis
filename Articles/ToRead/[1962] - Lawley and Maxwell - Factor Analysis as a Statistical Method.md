[1962] - Lawley and Maxwell - Factor Analysis as a Statistical Method

[Bartlett - 1953] " Factor Analysis must be regarded as a natural development in a field in which large sets of correlated variates arise, as a means of examining and describing the internal structure of the covariates and correlation matrices concerned."

Make a comparison between Principal Component analysis and Factor Analysis. The former does not need any assumptions to be applicable to data (not even to have random variables). 
One of the major difference lies in the fact that Factor Analysis postulates an assumption of linearity on the covariates whereas PCA does not ! (PCA is essentially only empirical, and suffers from being dependent on the scale of the covariates.). This linearity assumption is testable ! (If rejected, should consider adding quadratic terms, interaction terms, ...).

Historical note : This article was published before the theory about treating the common factors as parameters. (They say that it leads to difficulties when the sample size goes to infinity and point out to another article Whittle-1953).

Only treats the loadings and the error terms as parameters.

The explicit the **Centroid Method** for estimating the factor model. It is essentially a geometrical method but which is quite arbitrary (make it difficult to analyse it statistically). In practice a unique solution is not always possible ! This method also depends on the scale of the covariates. We can then standardize the variance of the covariances but this apparently leads to difficulties when tests of significances are considered. But this method is still really fast (this should permits to get a first estimates for further more powerfull methods).


**Maximum Likelihood method** assumes the covariates to follow a multivariates normal distribution, othogonal factors, orthogonal errors.
We can then decompose the covariance matrix of the covariates. Thus giving us an hypothesis to be tested. 
Given the normality assumption, the covariance matrix of the covariates follows a Wishart distribution.

This article also state the rotational problem of the estimates. "[...] the maximum likelihood method, [...], leads to equations for estimating the "l" which are satisfied by an infinity of solutions" (p216). "The method determines the k-dimensional space in which the factors lie, but it cannot determine their directions in that space." (p216). This leaves the statistician the choice of choosing a particular solution ! They choose to have a particular matrix diagonal which fixes the matrix of loadings.

MLE are independent of the scale/metric of covariates, from the fact that a change of scale implies a rescaling of the appropriate loadings.

The fact that factors are not considered as parameters is not important for the decomposition of the covariance matrix. But if we want to still obtain estimates we first need to estimate the loadings and errors then regress those with the covariates to obtain the "estimated" factors. 

