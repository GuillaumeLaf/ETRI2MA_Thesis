[2015] Cho and Fryzlewicz - Multiple-change-point detection for high dimensional time series via sparsified binary segmentation.md

The basic idea is the segment time series.
 They introduce an algorithm for detecting muktiple change points in high dimenseional time series.
 
 The cross dimension and the sample size cannot diverge freely.
 
 Their method is sparse in the sens that they threshold a CUSUM (???) statistic for detecting change points. This thresholding reduces some difficulties in the high dimensional setting.
 
 They introduce the multivariate LSW model (extension of the bivariate of Sanderson 2010)
 
 CUSUM statistic gives us the likelyhood of a change point.
 
 They make assumptions on the number and behavior of change points in the time series (which are allowed to diverge with the sample size).
 
 Their definition of the multivariate LSW model is the same as in Sanderson (2010). The dependence structure of the time series is contained in the innovation process, not only in the wavelet coefficients. The innovations are however limited to be correlated for the same scale and time point. Innovations on different scales are not allowed to be correlated !
 
 For their purpose they change the formal definition of the wavelet periodogram to the difference between 2 raw wavelet coefficients.
 
 NOTE : at coarser scales, the raw wavelet coefficents exhibits higher levels of autocorrelation (due creasing length of the wavelet).
 
 The authors define the cross scale autocorrelation wavelets ! They only provide it to define differrently the inner product matrix.
 They don't correct the raw periodogram since they are only interested in the change points of the second order structure (analysed by their modified periodogram).
 
 
