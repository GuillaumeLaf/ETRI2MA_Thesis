[2010] Sanderson et al. - Estimating linear dependence between nonstationary time series using locally stationary wavelet model.md

"The coherence function is derived by normalizing the cross-spectrum by the individual spectra and [...] measures the correlation between the signals as a function of frequency".

This paper propose a "locally stationary wavelet coherence" based on the LSW model of Nason et al. (2000).

The main difference with their coherence formulation is that it estimates the dependence structure between innovations of each process, without being contaminated by the dependence within each series. 

The main quantity of interest is the dependence measure between the innovations processes (rho) (=LSW coherence), which is different from the cross-correlation (between the two series).
The innovation processes are only allowed to be correlated on the same scale and at the same time (no dependence between innovation at different scales).

errors are normally distributed.

The wavelet spectrum quantifies the contribution to the variance of the process of the scale "j" and rescaled-time "k/T".

From the definition of the cross-spectrum, a change in the latter can come from a change in the individual wavelet spectrum or a change in dependency between innovation processes. The cross-spectrum can therefore not be used alone to quantify the coherences. 

Wavelet really make everything time dependent. Hence the coherence also become time varying. 

The autocorrelation wavelets in the coherence formula have the same role as the complex exponential in Fourier. However, they have a bounded support which make the coherence local. 

Practical considerations : The estimators can be unstable. They could output non-positive values for the specta (which is not possible). 
They recommend smoothing along scales in addition to time. This will introduce some bias but we can limit this bias. This additional smoothing also reduces the variance of the estimator further. 
