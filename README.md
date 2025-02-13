## Motivation

Previous attempt for optimizing parameters for neural mass mdoels (NMMs) using MCMC approach, showed that HMC-E is statistically more efficient than LMC-R (Sengupta et al., 2016). 
Recently, Baldy et al., (2024) used several probabilistic programming languages for DCM model inversion in neurobiologically plausible generative models, and reported that model inversion with gradient-based Markov Chain Monte Carlo outperformed than variational approximation frameworks; 
especially, posterior estimation using a self-tuning variant of Hamiltonian Monte Carlo and the automatic Laplace approximation. PyMC is a powerful probabilistic programming package, implementing HMC using No-U-Turn Sampler (NUTS; Hoffman, 2014). Here, we tried to test the predictive accuracy of PyMC for DCM in fMRI bold times series.

