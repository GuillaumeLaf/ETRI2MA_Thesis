[1995] Nason and Silverman - The stationary wavelet transform and some statistical applications

This paper constitutes a 'tutorial' for both the standard wavelet transform and the stationary wavelet transform. 
The main difference lies in the fact that the latter uses non-decimated wavelets.
This leads the latter to redundancies in the representation.

The authors note that "the stationary wavelet transform has a valuable role in the exploration and spectral analysis of non-stationary time series".

This paper uses "periodic boundaries conditions" for the treatments of boundaries in the convolution (in accordance with fourier analysis).

The recall the notion of *Quadrature mirror filters* which are filters satisfying several conditions (internal and mutual orthogonality and normalization).
There exists some methods to construct such pairs of filters (see Daubechie, ...).

They use the Daubechie 6 for their examples.
They assume data length of power of 2.

Following Multiresolution Analysis, they define the smooth and detail coefficients of the decomposition recursively. Note that the smooth coeffs. are obtain from the low pass filter "h". Conversely, the details coeffs are obtain via the high pass filter.

The fact that the DWT is orthogonal, we are basically choosing a particular basis for the space R^n.
We can slightly modify the DWT to obtain some other choice of basis. For instance they point out to the **"curtailed DWT"**, which correspond to stopping the decomposition before attaining the maximum level of decomposition permitted by the length of the signal. 

The DWT could also be modified by changing the decimating operator, instead of taking every even index we could use every odd index for the decimation. Note that the result will not be the same (since we are not using the same basis) but the transformation is still orthogonal and we can still carry out a multiresolution analysis.

We can even alternate between the choice of decimating operator for different scale (we inverse the transform by using the corresponding inverse operators). Each sequence of choice will give us a different result (since it is a different basis). The authors call this transform, the **"epsilon-decimated DWT"**.

