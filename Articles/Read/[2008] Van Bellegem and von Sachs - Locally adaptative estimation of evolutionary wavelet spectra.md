[2008] Van Bellegem and von Sachs - Locally adaptative estimation of evolutionary wavelet spectra.md

"non-parameteric regression, for which "asymptotic" means an ideal  knowledge about the local structure of the underlying curve."

"Because wavelets system are well localied in time and frequency, they appear more natural for modelling the time-varying spectra of non stationary processes."

The authors extend the model of Nason et al. (2000) to account for discontinuities in the wavelet spectrum (non-lipschitz behavior).

They use an exponential inequality from Dahlhaus and Polonik (2002) which is important for the proofs in this articles.

They change the Lipschitz condition on the spectrum (Nason et al. 2000) to a total variation condition. 
They recall that the coefficients of the SWT are not uniquely identified. "[...] the model allows the asymptotic identification of the model coefficients determined by uniquely defined W^2(z) (spectrum).

In the proof of Proposition 1, I don't understand the where the total variation comes from. From thinking a bit more, I found that they partition an integral into a discrete sum of smaller integrals and switch the sum and integrals to find the TV. The latter is independent of "z" thus the smaller integral contains a constant.

Since the autocorrelation wavelet is a wavelet, then it allows to have a multiscale decomposition of the autocovariance structure.

The remind the fact that we could not obtain a wavelet-type evolutionary spectrum with decimated wavelets (which would give us an identity for the correction matrix "A").

## Their estimator 
It is essentially an average of the wavelet periodogram over an interval in time. 
Note that the added an noise process in their estimator fo the sake of regularization. The process X may not be invertible (non-finite spectrum). Doing so has no effect on the bias since the estimator is an average (over zero-mean additive noise process). 

They prove the usual convergence for their estimator : expectation and variance; and their rate of convergence. In the proofs they use results from other papers about bounding quadratic random variables. 

Note that the variance of their estimator does not tend to zero asymptotically. Their estimator is "non-degenerate". (They need an additional assumption for the exponential inequality) (something has to grow with T). Only then they prove the consistency. 
The intuition behind this additional growing term give us the following interpretation : As more observations become available, the probability of observing increasingly large deviation tends to zero. 

The next big proof is about the choice of smoothing window for the average. They chose an adaptative-method. 
This choice of window length is based on an probability exponentional upperbound. The latter gives us the possibility to test. (They call it the "homogeneity test").
