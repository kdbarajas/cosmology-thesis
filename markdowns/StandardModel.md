------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...

# Introduction to Modern Cosmology & Large Scale Structure Formation

The Lambda Cold Dark Matter ($\Lambda\text{CDM}$) model of cosmology is the strongest model for describing the past and future of the Universe and is predicated on the fundamental assumptions of the Cosmological Principle: that the Universe on large scales is isotropic and homogeneous. The importance of this assumption cannot be understated as the metric that follows from the model provides the basis for our understanding of the evolution and growth of structure in the Universe. Within this framework, measurements from galaxy rotations, the cosmic microwave background radiation, Type Ia supernovae, and big bang nucleosynthesis strongly support the need for both dark matter and dark energy to describe a universe that adheres to the Cosmological Principle. And, while the model tells us about the density composition of the Universe it leaves much to be desired in our fundamental understanding of dark matter and dark energy, which together compose the vast majority of the known Universe. 

We can investigate these mysterious phenomenon through peculiar velocity and redshift surveys which use galaxies as tracers of the underlying density field that is predominately formed by dark matter. Thus, by analyzing large scale motion in the local Universe we can test paradigms set forth by the $\Lambda\text{CDM}$ model. Peculiar velocities thus serve as an interesting probe that may lead to new insight into the inner workings of the Universe, in particular where inconsistencies arise. One such instance is that of recent findings of large-scale bulk flows which may indicate an excess of structure formation on scales where the Universe is expected to be fairly uniform in contradiction with the standard model. Characterizing the strength of the density perturbations on large scales that may lead to an excess of power may provide insight into these findings.

In the first section we provide the theoretical foundation of modern cosmology: Einstein's theory of general relativity, the FLRW metric, and the Friedmann equation for an evolving universe. In the second section we 

## General Relativity & Einstein's Field Equations

- General relativity can be seen as the generalization of Newtonian gravity to a relativistic spacetime geometry.

- Using spacetime coordinates $(ct, x, y, z)$ to describe events.

  - where we define separation between two events by the line segment $ds^2 = -c^2 dt^2 + dx^2 + dy^2 + dz^2 \equiv g_{\mu\nu}dx^\mu dx^\nu$, an invariant quantity under coordinate transformation\footnote{This means that from any inertial frame of reference, an observer would measure the same separation $ds$.}

- Einstein's Field Equations:
  $$
  G^{\mu\nu} = \frac{8\pi G}{c^4} \left( T^{\mu\nu} + T_{\text{vac}}^{\mu\nu} \right) = \frac{8\pi G}{c^4} T_{\text{all}}^{\mu\nu}
  $$
  {#eq:EFE}

  - Left side represents a second-rank tensor that describes the curvature of spacetime.

  - Right side represents the stress-energy tensor $T_{\text{all}}^{\mu\nu}$ for the total matter and energy in the Universe. The first term represents the stress-energy $T^{\mu\nu}$ for a perfect fluid associated with a homogeneous and isotropic Universe. The second term represents the stress-energy for a vacuum that acts a repulsive pressure that counteracts gravitational attraction,
    $$
    T_{\text{vac}}^{\mu\nu} = - \frac{\Lambda c^4}{8\pi G} g^{\mu\nu}
    $$
    where $\Lambda$ represents the cosmological constant providing the best account for dark energy in the $\Lambda\text{CDM}$ model.

### Friedmann-Lemaitre-Robertson-Walker Metric

- The FLRW metric for a homogeneous and isotropic Universe is given by
  $$
  ds^2 = -c^2dt^2 + a(t)^2 dr^2
  $$
  where $a(t)$ represents the scale factor and the distance $r$ describes the comoving radial distance between two galaxies independent of cosmic expansion over any 3-dimensional coordinate space.

- The FLRW metric takes the standard form in hyperspherical coordinates
  $$
  ds^2 = -c^2dt^2 + R(t)^2 \left[  d\chi^2 + S_K(\chi)^2 \,  d\Omega^2   \right]
  $$

  - where $R(t)$ is the time-dependent radius of the Universe, $\chi$ is a dimensionless radial coordinate, and $d\Omega$ is the spherical coordinate space corresponding to $d\theta^2 + \sin^2 \! \theta \, d\phi^2$.

  - The radius $R(t)$ is related to the scale factor by $R(t) \equiv R_0 \, a(t)$ with a radius of curvature $R_0 = (\sqrt{|K|})^{-1}$ where $K$ is the curvature constant.  The physical comoving distance coordinate $\bar{r}$ can be related to the dimensionless comoving angular coordinate $\chi$ by $\bar{r} = R_0 \chi$. The geometry of the Universe $S_\kappa(\chi)$ depends on the curvature $K$ such that
    $$
    S_K(\chi) =
    \begin{cases}
    \sin^2 \! \chi & \text{for } \ K > 0 \hspace{5mm} \text{ (open `spherical' universe),}\\
    \chi & \text{for } \ K = 0 \hspace{5mm}  \text{ (flat universe)},\\
    \sinh^2 \! \chi & \text{for } \ K < 0 \hspace{5mm} \text{ (closed `hyperbolic' universe).}
    \end{cases}
    $$

  - Observations from the CMB amongst others strongly support a infinitely flat Universe such that $K \simeq 0$ and $R \to \infty$.

  ### Hubble Flow

- As before, the comoving distance coordinate $\bar{r}$ describes the distance between two galaxies independent of cosmic expansion. The 'true' physical distance $d$, otherwise known as the proper distance, is the physical separation an observer at rest with respect to cosmic expansion would observe a distant galaxy and is dependent on the scale factor such that  $d(t) = a(t) \, \bar{r}$. The cosmic expansion velocity $v$ (more commonly known as the Hubble flow) can therefore be deduced from the rate of change of the separation distance such that
  $$
  v \equiv \dot d = \frac{\dot a}{a} \, d = H(t) \, d
  $$
  {#eq:expansionvelo}

  where
  $$
  H(t) \equiv \frac{\dot a}{a}
  $$
  {#eq:hubbleparam}

  represents the time-dependent Hubble parameter. At present, $H$ is known as the Hubble constant $H_0$ and is defined by $H_0 \equiv \dot a_0 / a_0 = \dot a_0$ (normalized to $a_0 =1$ at present-time). In practice, the value of the Hubble constant is most usefully written as $H_0= 100\, h\,$\si{\km\per\s\per\Mpc} in terms of the dimensionless parameter $h$ defined by the current accepted value. 

  ### Cosmological Redshift


- In practice, the only meaningful way in which we can measure the cosmological expansion velocity is by measuring the redshift. We can relate the cosmological redshift from @eq:redshift to the scale factor $a$ of the Universe by
  $$
  z_\text{cos} \equiv \frac{\lambda_\text{obs} - \lambda_\text{em}}{\lambda_\text{em}} = \frac{a_0}{a_\text{em}}-1  = \frac{1}{a_\text{em}} -1
  $$
  {#eq:cosredshift}

- where the present scale factor is given by $a_0 = a(t_\text{rec}) = 1$  corresponding to the time of observation $t_\text{rec}$ while $a_\text{em} = a(t_\text{em})$ is the the scale factor at the time of emission $t_\text{em}$.

 - In the low-redshift limit, we can approximate @eq:expansionvelo as Hubble's law by Taylor expanding $a_\text{em}= a(t_\text{rec} - \Delta t)$ about $a_0$ such that $a_\text{em}  \simeq 1 - \dot a_0 \, \Delta t$ is the first-order approximation where $\Delta t = t_\text{rec} - t_\text{em}$. Then by using the definition of the Hubble constant and the binomial approximation we can rewrite @eq:cosredshift as
     $$
     z_\text{cos} \approx \dot a \, \Delta t = H_0 \, \Delta d/c \, .
     $$
     where $cz_\text{cos} \approx H_0 d$ is the approximate expansion velocity at present-time for $z \ll 1$.

     ### Friedmann Equation for an Evolving Universe


- Solving the EFEs using the FLRW metric provides the Friedman equation that model the time-evolution of a homogeneous and isotropic Universe:
  $$
  H^2 \equiv \left( \frac{\dot a}{a} \right)^2 = \left( \frac{8\pi G}{3} \right) \rho_\text{tot} - \frac{K c^2}{a^2}
  $$

  {#friedmann}

  where
  $$
  \rho_\text{tot} \equiv \frac{\rho_{m0}}{a^3} +\frac {\rho_{r0} }{a^4} + \rho_\Lambda
  $$
  {#eq:ptot}

  is the total energy density and $\rho_{m0}$ and $\rho_{r0}$ are the matter and radiation density at present and $\rho_\Lambda$ is the energy density due to the cosmological constant which is constant with time.


- We can define the _critical density_ $\rho_\text{crit}$ from the Friedmann equation as
  $$
  \rho_\text{crit} = \frac{3 H^2}{8\pi G}
  $$
  {#eq:pcrit}

  which when compared to the total density $\rho_\text{total}$ determines the type of spatial curvature of the Universe. If the total density equals the critical density than $K$ must be zero and the Universe has no spatial curvature indicating a flat spatial geometry. If the total density is less than the critical density than $K$ is negative implying a spherical geometry and if greater than the critical density than $K$ is positive implying a saddle-like geometry.

- We can compare the observed energy density $\rho_i$ to the the critical density by introducing a dimensionless ratio $\Omega_i \equiv \frac{\rho_i}{\rho_\text{crit}}$ known as the density parameter introduced in Section # such that at present-time @eq:friedmann becomes
  $$
  (\Omega_m + \Omega_r + \Omega_\Lambda )-1 = \frac{Kc^2}{H_0^2} \equiv \Omega_k
  $$
  where $\Omega_k$ is the curvature parameter and the density parameter of matter, radiation, dark energy, and the curvature are given by
  $$
  \Omega_m = \frac{8\pi G \rho_m}{3 H_0^2}, \quad \Omega_r = \frac{8\pi G \rho_\gamma}{3H_0^2}, \quad \Omega_\Lambda = \frac{\Lambda c^2}{3 H_0^2} \,.
  $$

- The best measurements of the CMB indicate that the total density $\Omega_0$ is at unity with the critical density such that
  $$
  \Omega_0 = \Omega_m + \Omega_\gamma + \Omega_\Lambda + \Omega_k \simeq 1
  $$
  where the curvature parameter $\Omega_k \simeq 0$.

- Finally, if we express the Friedmann equation in terms of the density parameters and use the definition of the Hubble parameter then 
  $$
  \left( \frac{da}{dt} \right)^2 = H_0^2 \left( \frac{\Omega_m}{a} + \frac{\Omega_\gamma}{a^2} + \Omega_\Lambda \, a^2 + \Omega_k 	\right)
  $$
  is the cosmological equation of motion that describes the evolution of the Universe based on the current expansion rate $H_0$, the individual mass-energy densities $\Omega_i$, and the spatial curvature $K$.

## Gravitational Instability Theory and the Growth of Structure

- While the Universe on very large scales is both isotropic and homogeneous, the tiny temperature fluctuations seen in the cosmic microwave background reflect the dawn of structure formation in the early Universe.



- These fluctuations reflect the growth of density perturbations in the primordial matter density field as matter attracted into over-dense regions known as gravitational instability theory. From the cosmological principle of isotropy and homogeneity, we assume that the initial density perturbations and the underlying density field were approximately Gaussian distributed.

- Thus, the first-order density perturbation term $\delta$  of a uniform matter density field $\rho$ is given by
  $$
  \rho(\textbf{r}) = \bar\rho (1 + \delta(\textbf{r}))
  $$
  where $\bar \rho$ is the average matter density and $\textbf{r}$ is the comoving distance coordinate such that the density perturbation can be expressed in the more common form
  $$
  \delta(\textbf{r}) =\frac{\rho(\textbf{r}) - \bar\rho }{\bar\rho}\, .
  $$

- We can express the matter density perturbation $\delta(\textbf{r})$ in Fourier space as $\delta(\textbf{k})$ where
  $$
  \delta(\textbf{r}) = \int d^3k \ \delta(\textbf{k})\exp(i\textbf{k} \cdot \textbf{r}) \quad\text{and}\quad \delta(\textbf{k}) = \int d^3k \ \delta(\textbf{k})\exp(i\textbf{k} \cdot \textbf{r}) \, .
  $$
   where $\textbf{k}$ is the wave vector related to the wavenumber by $\textbf{k} = k\ \hat{ \textbf{k}}$ with $k = \frac{2 \pi}{r}$.  Similar to the density field, we can describe a velocity field and its Fourier transform as
  $$
  \textbf{v}(\textbf{r}) = \int d^3k \ \textbf{v}(\textbf{k})\exp(i\textbf{k} \cdot \textbf{r}) \quad\text{and}\quad \textbf{v}(\textbf{k}) = \int d^3k \ \textbf{v}(\textbf{k})\exp(i\textbf{k} \cdot \textbf{r}) \, .
  $$
  {#velotransform}

- In linear theory, the velocity field is directly related to the underlying matter density field through the continuity equation\footnote{Provide continuity equation. Fluid in gravitational field. Conservation of mass. Dependent on the dynamics of the fluid such as density, pressure, and velocity distribution.} such that
  $$
  \textbf{v}(\textbf{k}) = - \frac{iH_0f}{k^2} \textbf{k} \, \delta(\textbf{k})
  $$
  {#eq:continuity}

  where $f$ is the growth rate of the linear growth factor $D(t)$ of density perturbations such that
  $$
  f = \frac{d \ln D(t)}{d \ln a} \simeq \Omega_m^\gamma
  $$
  and $\gamma$ is the growth index which is dependent on the model. Since the growth rate $f$ is driven by gravitational attraction, we often find it more intuitive to parameterize it in terms of the total matter density $\Omega_m$ since dark energy is not influenced by gravity with $\gamma \approx 0.55$ for a spatially flat universe (as predicted by GR and the $\Lambda\text{CDM}$ model). Similarly, we can express @eq:continuity in terms of the spatial velocity field $\textbf{v}(\textbf{r})$ and the density perturbations $\delta(\textbf{r})$ such that
  $$
  \textbf{v}(\textbf{r}) = \frac{H_0 f}{4\pi} \int d^3\textbf{r}^\prime \frac{\delta(\textbf{r}^\prime)(\textbf{r}^\prime - \textbf{r})}{|\textbf{r}^\prime - \textbf{r}|^3}\,
  $$
  where it becomes more obvious that peculiar velocities are a strong probe of structure on any scales due to being highly sensitive to perturbations of the underlying density field.

  ​

- Density field power spectrum assuming a linear evolution is given by
  $$
  \left<  |\delta(\textbf{k})|^2 \right> \equiv P(k)
  $$
  {#eq:densityps}

  ​

  Velocity field power spectrum
  $$
  P_v(k) \equiv \left<  |v(\textbf{k})|^2  \right> = \left( \frac{H_0 f}{k} \right)^2 P(k)
  $$
  {#eq:velocityps}

- The velocity power spectrum is a complete statistical description of peculiar velocities on linear scales where density perturbations are Gaussian.

