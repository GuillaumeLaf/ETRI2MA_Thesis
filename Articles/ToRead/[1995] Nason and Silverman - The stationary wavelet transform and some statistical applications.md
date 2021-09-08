[1995] Nason and Silverman - The stationary wavelet transform and some statistical applications

This paper constitutes a 'tutorial' for both the standard wavelet transform and the stationary wavelet transform. 
The main difference lies in the fact that the latter uses non-decimated wavelets.
This leads the latter to redundancies in the representation.

The authors note that "the stationary wavelet transform has a valuable role in the exploration and spectral analysis of non-stationary time series".

This paper uses "periodic boundaries conditions" for the treatments of boundaries in the convolution (in accordance with fourier analysis).

They recall the notion of *Quadrature mirror filters* which are filters satisfying several conditions (internal and mutual orthogonality and normalization).
There exists some methods to construct such pairs of filters (see Daubechie, ...).

They use the Daubechie 6 for their examples.
They assume data length of power of 2.

Following Multiresolution Analysis, they define the smooth and detail coefficients of the decomposition recursively. Note that the smooth coeffs. are obtain from the low pass filter "h". Conversely, the details coeffs are obtain via the high pass filter.

The fact that the DWT is orthogonal, we are basically choosing a particular basis for the space R^n.
We can slightly modify the DWT to obtain some other choice of basis. For instance they point out to the **"curtailed DWT"**, which correspond to stopping the decomposition before attaining the maximum level of decomposition permitted by the length of the signal. 

The DWT could also be modified by changing the decimating operator, instead of taking every even index we could use every odd index for the decimation. Note that the result will not be the same (since we are not using the same basis) but the transformation is still orthogonal and we can still carry out a multiresolution analysis.

We can even alternate between the choice of decimating operator for different scale (we inverse the transform by using the corresponding inverse operators). Each sequence of choice will give us a different result (since it is a different basis). The authors call this transform, the **"epsilon-decimated DWT"**.

They show that the basis vectors of the "espilon-decimated DWT" can be obtained from those of the standard DWT by applying a particular shift operator to the original signal.

Next they demysified the **"Continuous Wavelet Transform"**.
They remind the *scaling function* in multiresolution analysis. This function is also known as the father wavelet. It depends on the low pass filter "h".
Conversely, the *mother wavelet* depends on the high-pass filter "g".

The filters "h" and "g" are exactly the same as in the multiresolution analysis. In other words, in wavelet theory we need special functions (father and mother wavelets) which depends on some coefficients in the linear combination property. And it turns out that the quadrature mirror filters are exactly the required coefficients. Consequently, we can perform a multiresolution analysis of any function in L2 with those father and mother wavelets (dilated and translated).

The detail coefficients gives information about the function at a particular scale and near a point in time-domain.

The **Stationary Wavelet Transform** is a modification of the DWT which does not depend on the sequence of decimating operator. The SWT does not decimate and produce sub-sequences of the same length as the original signal. It modify the filters at each level by adding zeros in-between previous elements of the filter. The SWT contains the coefficients of the espilon-decimated DWt for every choice of espilon. 

The SWT coeffs are not characterized by a given basis but a collection of basis (since SWT is not orthogonal).Therefore, inversing the transform is not unique ! If the inverse transform is used with an exact SWT then all possible inversion will give the same result. But if we modify the estimated coefficients (thresholding, ...) then the reconstructed signal will be dependent on the inversion method used. 

The **epsilon-basis inverse** of the SWT corresponds to selecting the some coefficients (as in the epsilon-decimation) and making an inverse DWT with those coeffs (for the particular choice of epsilon sequence).

The **average basis inverse** corresponds to averaging the inverse of all possible epsilon-basis inverse. The authors made a comment about the time complexity of this algorithm which is not as complex as it seems. 

Application to nonparametric regression : 
To estimate an unknown function with additive error, use the DWT then apply a thresholding methods to the estimated coefficients then revert the transform to get an estimate of the true function. 
We can use the SWT to do the same thing. However, we have to choose a particular basis for inverting the transform. This problem of "best basis" is a binary tree (at each level of decomposition we have to choose whether to use the odd or even coefficients). We can use an entropy function to choose between cases. This problem can be turned into a dynamic programming problem. 
We can also use the averaging basis for getting an estimate of the function.

Recall, in stationary time series, the periodogram is defined to be the squared modulus of the discrete Fourier Transform. By analogy the **wavelet periodogram** is the squared coefficients.
If the original process is stochastic and gaussian then the periodogram will be chi-squared distributed (since the wavelet coefficients depends linearily on the original time series). As in classical stationary time series, the periodogram is not a consistent estimator of the spectrum. 

They briefly discuss the **local autocovariance**.
(((side note : The Wigner distribution function provides the highest possible temporal vs frequency resolution which is mathematically possible within the limitation of the uncertainty principle.))). The wavelet spectrum can be defined in terms of the Wigner distribution. This function is also simply the local spectrum of the Fourier transform of the local autocovariance. 

**I haven't quite understood pages 294 and 295 about the behavior of the wavelet spectrum/periodogram with a perfect sine wave signal.**

