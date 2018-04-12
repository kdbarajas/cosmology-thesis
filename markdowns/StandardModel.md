------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...

# Modern Cosmology & Large Scale Structure Formation

The Lambda Cold Dark Matter ($\Lambda\text{CDM}$) model of cosmology is the strongest model for describing the past and future of the Universe and is predicated on the fundamental assumptions of the Cosmological Principle: that the Universe on large scales is isotropic and homogeneous. The importance of this assumption cannot be understated as the metric that follows from the model provides the basis for our understanding of the evolution and growth of structure in the Universe. Within this framework, we find the need for both dark matter and dark energy in order to describe a universe that adheres to the Cosmological Principle, but the model leaves much to be desired in our understanding of their fundamental nature. One possible way of probing these phenomenon is by testing the $\Lambda\text{CDM}$ paradigm in search of deviations from the model that may provide a glimpse to the inner workings of the Universe.

## General Relativity & Einstein's Field Equations

- General relativity can be seen as the generalization of Newtonian gravity to a relativistic spacetime geometry.

- Using spacetime coordinates $(ct, x, y, z)$ to describe events.

  - where we define separation between two events by the line segment $ds^2 = -c^2 dt^2 + dx^2 + dy^2 + dz^2 \equiv g_{\mu\nu}dx^\mu dx^\nu$, an invariant quantity under coordinate transformation\footnote{This means that from any inertial frame of reference, an observer would measure the same separation $ds$.}

- Einstein's Field Equations:

- $$
  G^{\mu\nu} = \frac{8\pi G}{c^4} \left( T^{\mu\nu} + T_{\text{vac}}^{\mu\nu} \right) = \frac{8\pi G}{c^4} T_{\text{all}}^{\mu\nu}
  $$

  - Left side represents a second-rank tensor that describes the curvature of spacetime.

  - Right side represents the stress-energy tensor $T_{\text{all}}^{\mu\nu}$ for the total matter and energy in the Universe. The first term represents the stress-energy $T^{\mu\nu}$ for a perfect fluid associated with a homogeneous and isotropic Universe. The second term represents the stress-energy for a vacuum that acts a repulsive pressure that counteracts gravitational attraction,

  - $$
    T_{\text{vac}}^{\mu\nu} = - \frac{\Lambda c^4}{8\pi G} g^{\mu\nu}
    $$

    where $\Lambda$ represents the cosmological constant providing the best account for dark energy in the $\Lambda\text{CDM}$ model.

## Friedmann-Lemaitre-Robertson-Walker Metric

- The FLRW metric for a homogeneous and isotropic Universe is given by

- $$
  ds^2 = -c^2dt^2 + a(t)^2 dr^2
  $$

  - where $a(t)$ represents the scale factor and the distance $r$ describes the comoving radial distance between two galaxies independent of cosmic expansion over any 3-dimensional coordinate space.

- The FLRW metric takes the standard form in hyperspherical coordinates

- $$
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

  - $$
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

 -  In the low-redshift limit, we can approximate @eq:expansionvelo as Hubble's law by Taylor expanding $a_\text{em}= a(t_\text{rec} - \Delta t)$ about $a_0$ such that $a_\text{em}  \simeq 1 - \dot a_0 \, \Delta t$ is the first-order approximation where $\Delta t = t_\text{rec} - t_\text{em}$. Then by using the definition of the Hubble constant and the binomial approximation we can rewrite @eq:cosredshift as 

     -  $$
        z_\text{cos} \approx \dot a \, \Delta t = H_0 \, \Delta d/c \, .
        $$


    where $cz_\text{cos} \approx H_0 d$ is the approximate expansion velocity at present-time for $z \ll 1$.

### Friedmann Equation for an Evolving Universe

- Solving the EFEs using the FLRW metric provides the Friedman equation that model the time-evolution of a homogeneous and isotropic Universe:
  $$
  H^2 \equiv \left( \frac{\dot a}{a} \right)^2 = \left( \frac{8\pi G}{3} \right) \rho_\text{tot} - \frac{K c^2}{a^2}
  $$

  - {#friedmann} where

  - $$
    \rho_\text{tot} \equiv \frac{\rho_{m0}}{a^3} +\frac {\rho_{r0} }{a^4} + \rho_\Lambda
    $$

  - is the total energy density and $\rho_{m0}$ and $\rho_{r0}$ are the matter and radiation density at present and $\rho_\Lambda$ is the energy density due to the cosmological constant which is constant with time.


- We can define the _critical density_ $\rho_\text{crit}$ from the Friedmann equation as

- $$
  \rho_\text{crit} = \frac{3 H^2}{8\pi G}
  $$

  which when compared to the total density $\rho_\text{total}$ determines the type of spatial curvature of the Universe. If the total density equals the critical density than $K$ must be zero and the Universe has no spatial curvature indicating a flat spatial geometry. If the total density is less than the critical density than $K$ is negative implying a spherical geometry and if greater than the critical density than $K$ is positive implying a saddle-like geometry.

- We can compare the observed energy density $\rho_i$ to the the critical density by introducing a dimensionless ratio $\Omega_i \equiv \frac{\rho_i}{\rho_\text{crit}}$ known as the density parameter introduced in Section # such that at present-time @eq:friedmann becomes

- $$
  (\Omega_m + \Omega_r + \Omega_\Lambda )-1 = \frac{Kc^2}{H_0^2} \equiv \Omega_k
  $$

  where $\Omega_k$ is the curvature parameter and the density parameter of matter, radiation, dark energy, and the curvature are given by
  $$
  \Omega_m = \frac{8\pi G \rho_m}{3 H_0^2}, \quad \Omega_r = \frac{8\pi G \rho_\gamma}{3H_0^2}, \quad \Omega_\Lambda = \frac{\Lambda c^2}{3 H_0^2}
  $$

- The best measurements of the CMB indicate that the total density $\Omega_0$ is at unity with the critical density such that

- $$
  \Omega_0 = \Omega_m + \Omega_\gamma + \Omega_\Lambda + \Omega_k \simeq 1
  $$

  where the curvature parameter $\Omega_k \simeq 0$.

- Finally, if we express the Friedmann equation in terms of the density parameters and use the definition of the Hubble parameter then 

- $$
  \left( \frac{da}{dt} \right)^2 = H_0^2 \left( \frac{\Omega_m}{a} + \frac{\Omega_\gamma}{a^2} + \Omega_\Lambda \, a^2 + \Omega_k 	\right)
  $$

  is the cosmological equation of motion that describes the evolution of the Universe based on the current expansion rate $H_0$, the individual mass-energy densities $\Omega_i$, and the spatial curvature $K$.

- ​

### Peculiar Velocity

Hubble's law represents an empirical relationship for the expanding universe where each galaxy is static with respect to cosmological expansion. However, an ideal Hubble's law neglects gravitational attraction to higher density regions of space which induce 'peculiar' motion that deviates from cosmological expansion velocity $c z_\text{cos} = H_0d$ (also known as the Hubble flow). The consequence of a continuous inflow of matter towards these regions of space is a state of matter over-density known as gravitational collapse, which provides the means for the formation and growth of structure in the local Universe. 

Thus, measurements of peculiar velocity are a compelling cosmological probe of local structure and the nature of dark matter due to the motion of galaxies tracing the underlying matter density field.



We can estimate peculiar velocities as deviations within the observed redshift $z_{obs}$ from Hubble's law as a result of Doppler redshift $z_\text{doppler}$ due to local motion. Unfortunately we are observationally limited to receding and approaching wavelengths along the 1D line-of-sight component of a galaxy's full 3D peculiar velocity vector. Any transverse motion along the line-of-sight is far too small to be detected through spectroscopic measurements and thus we would also expect any contribution to the line-of-sight to be in the form of noise in the signal. Following @eq:Hubble, at low-redshift where $v \ll c$, the line-of-sight component of the peculiar velocity $v_p$ is given by the familiar form

$$v_p \approx cz_\text{obs} - H_0d$$ {#eq:pecveloapprox}

\noindent where $c$ is the speed of light, $z_\text{obs}$ is the observed redshift, and $H_0d$ is the cosmological expansion velocity at a given comoving distance\footnote{Comoving distance refers to the real distance between two objects at rest with respect to the Hubble flow. In simpler terms, comoving distance is the physical distance between two objects in the absence of cosmic expansion.} $d$\footnote{Davis et al shows that due to redshift not being an additive property this crude approximation is only accurate for $z_\text{obs} << 0.1$, but for the introductory purposes of this section we find this form more than sufficient. We will revisit this equation in Section 2.#}. Therefore given a distance indicator, the comoving distance $d$ can be measured independently from the observed redshift $z_\text{obs}$ allowing us to estimate the peculiar velocity. The most common form of distance indicators are the various standard candles introduced in Sec 1.# which unfortunately suffer from large uncertainties. In contrast to the high accuracy redshift measurements available, the uncertainty on distance estimators can be upwards of $\simeq 20\%$ which can lead to uncertainties in the peculiar velocity measurement on the order of the velocity itself. Typical peculiar velocity measurement are expected to be of order \SI{300}{km/s} while the errors scale largely with the distance of the galaxy such that uncertainty $\delta_{v_p}$ can be approximated by $\delta_{v_p} \approx 0.20 H_0 d$. Given the large uncertainties, peculiar velocity measurements must be estimated through statistical means thus requiring large velocity surveys with both distance and redshift measurements\footnote{In Section 2.# we will discuss an estimator method developed by Watkins & Feldman that provides a more accurate method of statistically estimating peculiar velocities.}.



- ​

  ### For next section on cosmology

  ​


$$
v_p \equiv \textbf{\textit{v}} \cdot \textbf{\hat{r}} = c \left ( \frac{z\text{obs} - z\text{cos}}{1 + z_\text{cos}}  \right)
$$

- $$
  1 + z = (1 + z_H)(1 + v_{pec}/c)
  $$

  ​





