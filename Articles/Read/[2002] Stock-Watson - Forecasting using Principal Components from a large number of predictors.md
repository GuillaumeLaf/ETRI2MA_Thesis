Stock and Watson (2002) : Forecasting using principal components from a large number of predictors

This article treats the forecasting of a single time series with help of factor models to enhance forecast precision. The basic idea is to estimate common factors and to run a linear regression with the desired time series and those factors. 
It also proves the convergence of estimated factors to the true common factors. 
This convergence also holds true under time-varying assumptions of factor loadings.

# Assumptions
+ Factors
  + bounded eigenvectors (?)
  + diagonal cov. matrix of factors
  + orthonormal loadings (> eigenvectors)
+ Error
  + short-memory process
  + bounded cross-covariance
  + bounded 4th moment (needed since we don't assume Gaussianity)
+ OLS-like estimator for forecast

# Identification of the model
The assumptions they use to identify the models are the following : 
+ ![\frac{\Lambda \Lambda}{N} \rightarrow I_{r}](https://latex.codecogs.com/gif.latex?%5Cfrac%7B%5CLambda%5E%7B%27%7D%20%5CLambda%7D%7BN%7D%20%5Crightarrow%20I_%7Br%7D)
+ ![E(F_{t}F_{t}^{'}) = \Sigma_{FF}](https://latex.codecogs.com/gif.latex?E%28F_%7Bt%7DF_%7Bt%7D%5E%7B%27%7D%29%20%3D%20%5CSigma_%7BFF%7D), a diagonal matrix.  
The first one restrict the rotation matrix to be orthonormal and the second one restrict it to be diagonal.

# Estimation
Non-linear least squares by solving with setting the derivatives of the objective to zero.


