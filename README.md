
## Background and Motivations

### Motivation for DCM in Layer fMRI


Dynamic Causal Modelling (DCM) is a hypothesis-testing framework for specifying models of effective connectivity among brain regions (Friston et al., 2003; Zeidman et al., 2019). Its application in fMRI has been widely used among cognitive and clinical neuroscience researchers to foster circuit-based understanding of mental constructs. Nowadays, advancements in high-resolution fMRI open new avenues for studying layered cortical circuits. Additionally, enhancing conventional DCM to capture layer-specific fMRI could become a compelling idea to testing layer-specific connections that support cognitive functions proposed by Predictive Coding theories. Notably, Heinzle et al., 2016 proposed extending traditional balloon models to include the effects of blood draining while working with layer fMRI.

### Motivation for Using HMC and PyMc Approach

On the other hand, previous attempts to optimize parameters for neural mass models (NMMs) using the MCMC approach showed that HMC-E is statistically more efficient than LMC-R (Sengupta et al., 2016). Recently, Baldy et al. (2024) used several probabilistic programming languages for DCM model inversion in neurobiologically plausible generative models and reported that model inversion with gradient-based MCMC performed as well as variational approximation frameworks, especially posterior estimation using a self-tuning variant of Hamiltonian Monte Carlo and the automatic Laplace approximation. 
Meanwhile, PyMC is a powerful probabilistic programming package that implements HMC using a No-U-Turn Sampler (NUTS; Hoffman, 2014). 


### Method

I will build a simple model with 2 nodes and 2 layers, I wrote ODE functions, iterate with Pytensor. Then, I will add noise to the observation designing priors (priors are not implemented for 2 layer).

![Picture2](https://github.com/user-attachments/assets/d2862da7-e19b-4797-a469-5a43378db0af)



### Conclusion

Together, we tried to test the predictive accuracy of PyMC for DCM in fMRI bold times series and replicate a two-layer DCM proposed by Heinzle et al., 2016, in Python (just for practice and better understanding of methods).

