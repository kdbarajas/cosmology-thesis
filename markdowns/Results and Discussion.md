

------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...



# Results and Discussion

- In this section we present the results of our power scaling method using the Cosmicflows-3 catalogue. We then compare our results to $\Lambda\text{CDM}$ predictions by comparing the power scaled likelihood peaks to the likelihood of the standard model given the velocity data and then by comparing the constraints on $\Omega_m$ and $\sigma_8$ from a marginalized likelihood analysis with and without power scaling the linear power spectrum $P(k)$.

  ## Marginalized Likelihood over $\sigma_*$

  - As previously mentioned in Sec #, we include the Gaussian distributed variance term $\sigma_*^2$ within @eq:covariance to account for the 1D velocity dispersion due to small-scale, non-linear motion in our error measurements. The value of $\sigma_*$ varies between galaxy surveys and is dependent on the underlying sample and the method of measurement and is typically on the order of $\sim 250-350$\si{\km\per\s}. While values for $\sigma_*$ have been constrained for individual surveys, fixing $\sigma_*$ can bias results towards models that favor the value chosen. Therefore, we leave $\sigma_*$ as a free parameter due to it also acting as an additional noise term that includes unaccounted for systematic errors which is particularly useful given that the CF3 is a compilation of various surveys. In order to calculate a maximum likelihood estimate independent of $\sigma_*$ we marginalize over the nuisance parameter between $0 < \sigma_* \leq 1000$\si{\km\per\s} using the method described in Section #.

  - We find that the inclusion of baryons in the parameterization of the power spectrum provided by Eisenstein & Hu (1998) to strongly influence both the shape and amplitude of the power spectrum on both small and large scales. Fixing parameters to the fiducial cosmology provided by the best-fitting values from _Planck_, we show our constrain on $\Omega_b$ using @eq:likelihood in Fig #.  

  - $\Omega_b$ causes problems with the model. Show 1D likelihood over $\Omega_b$ keeping other values constant. Show power spectrum with ratio between mle and std to show the need for power on large scales.

    ​

    ![ml_OmOb_standard](../images/ml_OmOb_standard.png)

    ![powerspectrum_Ob](/home/kdbarajas/GitHub/cosmology-thesis/images/powerspectrum_Ob.png)

    ![ml_Omsig8_peak1](/home/kdbarajas/GitHub/cosmology-thesis/images/ml_Omsig8_standard.png)

  ## Adding power on large-scales

  - Explain probing strength of density perturbations by scaling the power spectrum using the piecewise equation
    $$
    P(k) \propto k^{n_s} \, T^2(k)
    \begin{cases}
    X  & \text{for } k\leq k_\text{scale} \\[1.25ex]
    1 & \text{for } k > k_\text{scale}
    \end{cases}
    $$
    ![powerscaling_example](/home/kdbarajas/GitHub/cosmology-thesis/images/powerscaling_example.png)

  - Two dominant peaks. First at very large scales ~500 h-1 Mpc and second at 80 h-1 Mpc. 

  ![powerscaling](../images/powerscaling.png)

  ## MLE of Parameters

  - MLE with and without Power Scaling features. without adding power on large scales that the MLE is very inconsistent with the standard model. When adding the peaks in the power scaling likelihood that both values are consistent with standard model.

    ​

    ​


