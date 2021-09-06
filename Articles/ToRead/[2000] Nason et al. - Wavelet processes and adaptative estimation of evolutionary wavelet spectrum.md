[2000] Nason et al. - Wavelet processes and adaptative estimation of evolutionary wavelet spectrum

This is the main paper about the processes used to construct a factor model.

Generalize the Fourier representation of stationary stochastic processes to non-stationary ones. 
They characterize the autocovariance of the process via wavelets (similar to the spectrum representation in Fourier).

The second-order structure changes over time !

They propose a new process based on wavelets and constraint the model to be locally stationary via constraints on the model coefficients (and not on the covariances, as in Mallat et al. 1998). "[...] to permit identification and estimation of a wavelet spectrum from a single finite length stretch of the process X_t by restricting the time variation of the second-order structure of X_t".

They use non-decimated wavelets which are not orthogonal.

They define the LSW processes for length of power of 2. 

The LSW model does not contain the scaling coefficients of wavelet analysis. The latter are not required since they are asymptotically included by the sum of the details coefficients.

The LSW model includes all the "short-memory" processes. 

The LSW reprenstation gives access to the Evolutionary Wavelet Spectrum which quantify the "local power" (contribution to the variance of the process). 

I took some time understanding most of the proofs. For instance, I understand better why it is usefull to know if the model representation is unique, and if not why. In the present case, the model coefficients are not uniquely defined but the covariance structure is. The proofs also outlined the origin of the correction of the raw periodogram. 
However some proofs are still difficult to grasp. For example, the proof of inversion of the "A" operator remains a mystery (in particular Theorem 2).
The formula for the local autocovariance was probably discovered by playing around with the covariance of the process following the LSW model. The autocorrelation wavelet emerged then.

The asymptotic theory of estimation is made given Gaussian assumptions on the orthonormal increments, hence the process is gaussian.

They obtain a description of the process' variance by summing the smoothed (not corrected ??? I believe it should also be corrected) wavelet periodogram over the scales.

They recognize the fact that the estimate of the EWS could be used as input for other models. 



