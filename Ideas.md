This file contains my ideas concerning my work. They may totally be wrong but they will help me build my understanding of the subject.

+ In the LSW process, since the estimated wavelet coefficients are the result of a convolution between the original process and a wavelet. Theoretical analysis may be made simpler by Fourier analysis.

+ Most of the articles about the multivariate LSW model don't assume inter-scale dependence of the innovation terms. They are restricted to the Mv-LSW of order zero of Koch. They are thus only using autocorrelation wavelets for the correction of the periodogram (and not cross-correlation wavelets). Assuming as in the literature would simplify the construction of a factor model since the matrix used for the eigendecomposition will be a block matrix (and it is known that the eigs of a block matrix is equal to the eigs of each of the blocks).

+ Since the coefficients are not uniquely defined by the spectrum is, then I should try to work with the square root of the spectrum (cheat to recover the uniqueness).

+ find a way of correctly estimating a positive semi-definite matrix (since correcting the raw periodogram may lead to negative values of variances).