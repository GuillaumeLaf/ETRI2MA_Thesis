[2015] Gibberd and Nelson - Estimating Multi-resolution dependency graphs within the locally stationary wavelet framework.md

Try to sparsly model the dependency structure in the multivariate setting.

They use the multivariate LSW model introduced by Park et al. (2014). 
All the dependencies are summed up in the matrix of wavelet coefficients. The idiosyncratic increments are considered independent of scale, time and cross-section (they are truly idiosyncratic).

They introduce a new method for estimating the wavelet spectrum. The main drawback of the previous methods of estimation was the correction of the raw periodogram with the wavelet crosscorrelation matrix could lead to a negative values in the periodogram, which in turn leads to an estimator which does not produce a positive-semidefinite matrix.

Their estimator introduce a regularization term in the optimization problem which leads to a bias estimator (which may have a smaller variance than an unbiais one). 
The regularization constant (lambda, here) introduce sparcity (the large lambda, the sparser the correlation matrix).

This paper does not develop any proofs and does not dig into theoretical concerns. They only provide an example of applying the multivariate LSW to EEG data. They also point out a possible way of solving estimation issues (when the estimate is not a positive semidefinite matrix.)
