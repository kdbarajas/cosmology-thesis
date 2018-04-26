------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...



# The Cosmicflows-3 Database

- The Cosmicflows-3 (CF3) database is a compilation of combined redshift and distance surveys of the local Universe 
- For our study of peculiar velocities we will be using distance measurements from the \textit{Cosmicflows-3} (CF3) compendium, which is a collection of various observational surveys of 17,669 individual galaxies (see Fig. \ref{fig:CF3}) \cite{Tully2016:cf3}. Each galaxy distance is measured and calibrated amongst different sources and surveys such as Type Ia ![img](file:///home/kdbarajas/GitHub/cosmology-thesis/images/CF3.png?lastModify=1524706206)
- supernovae observations, infrared photometry of galaxy rotation,  Cepheid variables photometry, and estimating the tip of the red giant branch. The galaxies are organized into groups of similar distances; for example, the Virgo Cluster, the largest group, consists of 161 individual galaxy measurements. The compendium provides 11,508 groups organized in this manner, but nearly every group contain less than ten galaxies and 9804 groups are denoted as "singles" due to containing only one galaxy. Despite the limited amount of groups with more than two galaxies, this is a significant improvement to its predecessor \textit{Cosmicflows-2} which contained only 8,188 individual galaxy entries in total \cite{Tully2013:cf2}. The distances (and the observed redshift) provided by \textit{Cosmicflows-3} allows us to calculate the peculiar velocity for both individual galaxies as well as groups.

# Peculiar Velocity Statistics & Models

##Gaussian Peculiar Velocity Estimator

- From Sec # we can move towards a more accurate estimates of peculiar  velocities. An important limitation on Hubble's law from @eq:hubblelaw is that the radial velocity must be much less than the speed of light. Since the radial velocity is the sum of the cosmological expansion $H_0\, r$ and the peculiar velocity $v_p$, this places a few limitations on the quantities we can calculate. This is because we know that the radial velocity is proportional to the redshift in the spectra of a distant object, and thus if the observed redshift becomes too large then the approximation held by Eq. \ref{redshift-radialvelo} is no longer valid. Such calculations at high redshifts using this method thus inherently introduce distortions in the radial velocity, with estimates placing the limit on the redshift at $z < 2$ before corrections are needed \cite{Kaiser2015:PerturbLumDist+PecVelo}. Since radial velocity is also proportional to the distance of an object, the same reasoning can be used to set limits on the distance. Fortunately, in this thesis we will be working with scales well within the boundaries of $v \ll c$ and $z < 2$. I define these scales below explicitly in terms of distance and size.


- Given that redshift is not an additive property (as previously assumed in the low-redshift limit), the observed redshift $z_\text{obs}$ is actually given by
  $$
  (1 + z_\text{obs}) = ( 1 + H_0 r / c) ( 1 + v_p / c)
  $$
  such that the line-of-sight peculiar velocity is

$$
v_p = c \left ( \frac{z_\text{obs} - z_\text{cos}}{1 + z_\text{cos}}  \right)
$$

{#eq:pecvelo}

- where  $z_\text{cos} = H_0 r /c$  and the peculiar velocity is expected to be Gaussian distributed with $\left < v_p \right> = 0$. Due to the accelerating expansion of the Universe, at very high redshifts the observed redshift $z_\text{obs}$ must be modulated by the deceleration parameter $q_0$ which is given by

$$
z_\text{mod} = z \, [ 1 + 0.5 (1 - q_0)\, z - (1/6) (1 - q_0 - 3 q_0^2 +1)\, z^2] \, .
$$

​	We can then rewrite @eq:pecvelo as
$$
v_p \equiv \textbf{v} \cdot \hat{\textbf{r}} = c \left ( \frac{z_\text{mod} - z_\text{cos}}{1 + z_\text{cos}}  \right) \simeq c \left ( \frac{z_\text{mod} - z_\text{cos}}{1 + z_\text{mod}}  \right)
$$

- Since peculiar velocity measurements are determined from distance estimates by means of the distance moduli $\mu$ from Sec. ##, the errors are not only large but also maintains the undesirable trait of being non-Gaussian distributed. As discussed in Sec. #, our fundamental assumption on the initial density fluctuations being Gaussian also requires that the peculiar velocity be Gaussian distributed. Watkins & Feldman (2015) provide a Gaussian distributed estimator of peculiar velocities given by
  $$
  v_e = \frac{c z_\text{mod}}{(1 + z_\text{mod})} \log(cz_\text{mod}/H_0 r_e)
  $$
  with an uncertainty of $\delta v_e = cz_\text{mod} \delta \mu_e / ( 1 + z_\text{mod})$ where $\delta \mu_e$ is the uncertainty in the log distance measurement.

## Parameterization of the Power Spectrum

- We follow Eisenstein and Hu (1998) to model the power spectrum as an initial power law such that $P(k) \propto  k^n T^2(k)$ where $n$ is the spectral index and $T(k)$ is the transfer function fitted by
  $$
  \begin{split}
  T(q) & = \frac{L_0}{L_0 + C_0 q^2}, \\
  L(q) & = \log(2e + 1.8q), \\
  C(q) & = 14.2 + \frac{731}{1 + 62.5q} \, .
  \end{split}
  $$
  where we parameterize the transfer function by
  $$
  q = \frac{k}{h \ \text{Mpc}^{-1}} \cdot \left( \frac{\vartheta_{2.7}^2}{\Gamma} \right) \,.
  $$
  with the CMB temperature given by $T_\text{CMB} = 2.7\vartheta_{2.7}$\si{\kelvin} and we use the shape parameter  $\Gamma$ (which is $\Omega_m h$ in the zero-baryon limit). However, the baryonic density is non-negligible and so a more accurate fit that takes into account the effects of baryonic oscillations is given by
  $$
  \Gamma_\text{eff}(k) = \Omega_m h \left[ \alpha_\Gamma + \frac{1- \alpha_\Gamma}{1 + (0.43ks)^4} \right]
  $$
  where
  $$
  \begin{split}
  \alpha_\Gamma = & 1 - 0.328 \log(431 \Omega_m h^2) \, \frac{\Omega_b}{\Omega_m}\\
  & + 0.38 \log(22.3 \Omega_m h^2) \left( \frac{\Omega_b}{\Omega_m} \right)^2, \\
  s = & \frac{44.5 \,h \log(9.83/\Omega_mh^2)}{\sqrt{1 + 10(\Omega_bh^2)^{3/4}}} \, h^{-1}\text{Mpc} \,.
  \end{split}
  $$

- We normalize the linear  power spectrum to a sphere of radius $ R = 8h^{-1}\text{Mpc}$, the scale on which matter fluctuations become non-linear, such that that variance in a given volume $V$ becomes
  $$
  \sigma_8^2 = \int_0^\infty \frac{dk}{k} \Delta^2(k) \widetilde{W}^2(kR)
  $$
  where $\widetilde{W}(kR) =  \frac{3j_1(kR)}{kR} $ is the spherical top-hat window, $j_1$ is the first order spherical Bessel function $j_1(x) = (\sin x - x \cos x)/x^2$, and $\Delta^2(k)$ is the dimensionless power spectrum which at present-time (i.e. $z=0$) is related to the power spectrum by
  $$
  \Delta^2(k)|_{z=0} \equiv \frac{k^3}{2\pi^2} P(k) \,.
  $$

- The normalization amplitude $a_\text{norm}$ of the power spectrum is thus given by
  $$
  a_\text{norm} = \frac{\sigma_8^2}{ \int_0^\infty \frac{dk}{k} \Delta^2(k)|_{z=0} \, \widetilde{W}^2(kR)} \,.
  $$


### Velocity Covariance Matrix

- If we had a full 3D view of the velocity field we could make a straightforward measurement of the velocity correlation between galaxies, however we are observationally limited to the 1D radial component of the peculiar velocity. We use a theoretical velocity covariance matrix developed by Kaiser (1988) to characterize the growth of structure on large scales from perturbations in the matter distribution.


- Measurement of the 1D line-of-sight peculiar velocity for a galaxy $i$ can be expanded in Fourier modes via @eq:velotransform:
  $$
  S_i (\textbf{r}_0) = \textbf{v}(\textbf{r}_0 + \textbf{r}_i) \cdot \hat{\textbf{r}}_i = \int d^3 k \ \hat{\textbf{k}} \cdot \hat{\textbf{r}}_i \, v(\textbf{k}) \, \exp [ i \textbf{k} \cdot (\textbf{r}_0 + \textbf{r}_i) ]
  $$

  - where we have adopted the standard notation $S_i$ to represent the velocity data and $\textbf{r}_0$ is the relative position from which measurements of a galaxy's distance at $\textbf{r}_i$ are made.


- The covariance matrix is given by
  $$
  \begin{split}
  R_{ij} &  = \left<(\hat{\textbf{r}}_i \cdot \textbf{v}(\textbf{r}_i)\, (\hat{\textbf{r}}_j \cdot \textbf{v}(\textbf{r}_j) \right>  + (\sigma_{\text{obs},i}^2 + \sigma_{*,i}^2)\, \delta_{ij} \\
  & = \left< S_i S_j  \right> + \Sigma_{i}^2 \, \delta_{ij}
  \end{split}
  $$
  {#:eq:covariance}

  - where the noise term $\Sigma_{i}^2 = \sigma_{\text{obs},i}^2 + \sigma_{*,i}^2$ represents the sum of the observational uncertainties $\sigma_{\text{obs},i}$ and the 1D velocity dispersion term $\sigma_{*,i}$ that account for non-linear small-scale motions.

  - $\left< S_i S_j  \right>$ depends on the model and the relative position between galaxies $i$ and $j$ such that
    $$
    \left< S_i(\textbf{r}_i) S_j(\textbf{r}_j) \right>= \frac{H_0^2 f(\Omega_m)^2 a_\text{norm}}{2\pi^2} \int dk \, P(k) \, \mathcal{W}(\textbf{r}_i, \textbf{r}_j, k)
    $$
    {#eq:correlation}

    where $P(k)$ is the power spectrum of the density field defined in @eq:densityps and @eq:velocityps and $\mathcal{W}(\textbf{r}_i, \textbf{r}_j, k)$ is the tensor window function calculated from galaxy position given by

$$
\mathcal{W}(\textbf{r}_i, \textbf{r}_j, k) = \int \frac{d^2k}{4\pi} \, \exp(i \textbf{k} \cdot (\textbf{r}_i - \textbf{r}_j)) \, ( \hat{\textbf{r}}_i \cdot \hat{\textbf{k}}) \, ( \hat{\textbf{r}}_j \cdot \hat{\textbf{k}}) \,.
$$

​		{#eq:tensorwindow}

- Ma et al. (2011) provides an analytical form of @eq:tensorwindow that transforms the tensor window function using spherical harmonics such that
  $$
  \mathcal{W}(\textbf{r}_i, \textbf{r}_j, k) =  \frac{1}{3} \cos \alpha \, (j_0(k A) - 2j_2(kA)) + \frac{1}{A^2} j_2(kA) \, r_i \, r_j\sin^2\alpha
  $$
  {#eq:analytical}

  where $j_0$ and $j_2$ are spherical Bessel functions, $A = |\textbf{r}_i - \textbf{r}_j|$ is the radial separation distance, and $\alpha$ is the angle between $\textbf{r}_i$ and $\textbf{r}_j$.

- Finally, @eq:correlation and @eq:analytical suggests that the line-of-sight peculiar velocity dispersion for a given galaxy $i$ should be given by the 1D rms velocity $\sigma_{v,i}$ where
  $$
  \sigma_{v,i}^2 = \frac{1}{3}\frac{H_0^2 f(\Omega_m)^2 a_\text{norm}}{2\pi^2} \int dk \, P(k) \, .
  $$




### Maximum Likelihood Estimate

- Given the line-of-sight peculiar velocity vector $\pmb{S}= (S_i, \ldots, S_N)$ for a given observational dataset of $N$ galaxies, the probability of observing a given cosmological model is given by
  $$
  \mathcal{L}(\pmb{\theta}  \,| \,  \pmb{S}) = \frac{1}{{(2\pi)}^{N/2}  \, {\det(\textbf{R}(\textbf{r};\pmb{\theta}))}^{1/2}} \, \exp \left( -\frac{1}{2} \pmb{S}^T \textbf{R}^{-1} \pmb{S}  \right)
  $$
  {#eq:likelihood}

  where $\textbf{R}(\textbf{r};\pmb{\theta})$ is an $N \times N$ covariance matrix defined in @eq:covariance and the model parameter(s) $\pmb{\theta} =(\theta_i, \ldots, \theta_n)$  depend on the underlying cosmology. In Bayesian statistics, any information about the model parameter of interest $\theta_i$ is constrained by the likelihood where the maximum likelihood value corresponds to the parameter value that best supports the data. 


- Bayes' theorem states the posterior distribution, $p(\pmb{\theta} \, | \, \pmb{S})$, the conditional probability distribution a multi-parameter model given the data, can be expressed as
  $$
  p(\pmb{\theta} \, | \, \pmb{S}) 
  = \frac{p(\pmb{\theta}) \, p(\pmb{S} \, | \, \pmb{\theta})}{\int p(\pmb{\theta}) \, p(\pmb{S} \, | \, \pmb{\theta}) \, d\pmb{\theta}_{-i}}
  = \frac{p(\pmb{\theta}) \mathcal{L}(\pmb{\theta}  \,| \,  \pmb{S})}{p( \pmb{S} \, | \, \theta_i )}
  \propto p(\pmb{\theta}) \mathcal{L}(\pmb{\theta}  \,| \,  \pmb{S})
  $$
  where the expression is equal when a normalization constant is included in the right-most term and we have used the fact that $\mathcal{L}(\pmb{\theta}  \,| \,  \pmb{S}) \equiv p(\pmb{S} \, | \, \pmb{\theta})$ to relate Bayes' theorem to @eq:likelihood.

- If we assume the standard 'non-informative' prior $p(\pmb{\theta}) = \text{const.}$, then the marginal posterior distribution of $\theta_i$ is given by
  $$
  p(\pmb{S} \, | \, \theta_i) \equiv \mathcal{L}(\theta_i \, | \, \pmb{S}) \propto \int_{-\infty}^\infty \mathcal{L}(\pmb{\theta} \, | \, \textbf{S}) \, d\pmb{\theta}_{-i}
  $$
  {#eq:marginalization}

  where we have marginalized over nuisance parameter(s) giving us the likelihood of our model parameter of interest given the data.

- Even so, the marginal likelihood can rarely be calculated numerically but if $\mathcal{L}(\pmb{\theta} \, | \, \pmb{S})$ is Gaussian we can then calculate @eq:marginalization analytically using the definition of the Gaussian integral where
  $$
  \int_{-\infty}^\infty \mathcal{L}(\pmb{\theta} \, | \, \textbf{S}) \, d\pmb{\theta}_{-i} \equiv \int_{-\infty}^{\infty} A_x \, \exp \left( - \frac{(x-x_0)^2}{2 \sigma_x^2}   \right) dx = A_x \sqrt{2\pi \sigma_x^2}
  $$
  {#eq:gaussianintegral}

- The likelihood analysis is limited by the computationally intensive calculation of the inverse covariance matrix $\textbf{R}^{-1}$ and the limit of the exponential term as it approaches negative infinity for very large numbers. We can simplify the problem by working in terms of the loglikelihood, which can easily handle very large numbers, where we can express @eq:likelihood as
  $$
  \log\mathcal{L}(\pmb{\theta} \, | \, \pmb{S}) \propto -\frac{1}{2} \left( \pmb{S}^T \textbf{R}^{-1} \pmb{S} + \text{logdet}(\textbf{R})  \right)
  $$
  {#eq:loglike}

  where the expression is equal with the addition of a constant to the right-side that depends on the size $N$ of the dataset. We can then analytically calculate the log of the marginal probability distribution of $\theta_i$ by using both @eq:gaussianintegral and @eq:loglike to simplify our calculation such that
  $$
  \begin{split}
  \log \mathcal{L}(\theta_i \, | \, \textbf{S}) & \propto \log \left( \int_{-\infty}^\infty \mathcal{L}(\pmb{\theta} \, | \, \textbf{S}) \, d\pmb{\theta}_{-i} \right)
  \propto \log \left( \int_{-\infty}^\infty \exp \left( \log\mathcal{L}(\pmb{\theta} \, | \, \textbf{S}) - \log\mathcal{L}(\theta_i, \pmb{\hat\theta}_{-i} \, | \, \textbf{S})  \right) \, d\pmb{\theta}_{-i} \right) \\
  & = \log(A_{-i}) + \frac{1}{2}\log \left(2\pi\sigma_{-i}^2 \, \right)
  \end{split}
  $$
  where $\pmb{\hat{\theta}}_{-i}$ is the maximum likelihood estimate for the nuisance parameter(s) $\pmb{\theta}_{-i}$ equivalent to $x_0$ in @eq:gaussianintegral with $A_{-i}$ and $\sigma_{-i}^2$  being the amplitude and variance of the Gaussian distribution about $\pmb{\hat{\theta}}_{-i}$.

- Finally, the maximum likelihood estimate (MLE) $\pmb{\hat{\theta}}_i$ of our parameter of interest $\theta_i$ is given by 
  $$
  \pmb{\hat{\theta}}_i = \text{arg max } \mathcal{L} (\theta_i \, | \, \pmb{S}) = \text{arg max } \log\mathcal{L}(\theta_i \, | \, \pmb{S}) \, .
  $$
  which allows us to freely work with the likelihood or loglikelihood depending on which is most convenient.

- Given the velocity data we can run a likelihood analysis over the parameterization of the power spectrum and the covariance matrix by varying cosmological parameters.

## 