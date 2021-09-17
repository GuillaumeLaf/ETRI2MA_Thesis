[2005] Crowley - An intuitive guide to wavelets for economists.md

The article introduces the notion of wavelets. I didn't learn much. 

They explain the notion of wavelet packet which is basically aplying the transform even on the detail corfficients.
In general not much information is present in the transform of the detail coefficients. 
They also explain that we can pick the decomposition we want in the wavelet packet tree in order to reconstruct the signal with so e particular frequencies components. 
The wavelets which produce further decompositions of the details exhibit some oscillations but still have are considered as wavelets. The more we pass the remaining details in the decomposition, the more oscillation has the wavelet.

Their exists a theory for choosing the best minimal set of elements in the decomposition tree to best reconstruct the signal.
 ote that in preseerving the orthogonality of the transform the best basis should not have kverlapping components at different scales.
 
 They introduce the MODWT as a shit invariant and non orthogonal DWT. The transform is a zero-phase transfrom since features in th time domain are aligned with features in the transform.
 
 With the MODWT we can make a analysis of the variance and covariances of multiple series.
 
 Since we have an estimates of the variance via wavelets, we can plug this estimate in models which require the variance. The authors exemplify this fact by estimating the fractional degree of an ARFIMA.
 
 
