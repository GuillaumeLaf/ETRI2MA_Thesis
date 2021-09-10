[2008] Van Bellegem and von Sachs - Locally adaptative estimation of evolutionary wavelet spectra.md

"non-parameteric regression, for which "asymptotic" means an ideal  knowledge about the local structure of the underlying curve."

"Because wavelets system are well localied in time and frequency, they appear more natural for modelling the time-varying spectra of non stationary processes."

The authors extend the model of Nason et al. (2000) to account for discontinuities in the wavelet spectrum (non-lipschitz behavior).

They use an exponential inequality from Dahlhaus and Polonik (2002) which is important for the proofs in this articles.

They change the Lipschitz condition on the spectrum (Nason et al. 2000) to a total variation condition. 
They recall that the coefficients of the SWT are not uniquely identified. "[...] the model allows the asymptotic identification of the model coefficients determined by uniquely defined W^2(z) (spectrum).

In the proof of Proposition 1, I don't understand the where the total variation comes from. From thinking a bit more, I found that they partition an integral into a discrete sum of smaller integrals and switch the sum and integrals to find the TV. The latter is independent of "z" thus the smaller integral contains a constant.
