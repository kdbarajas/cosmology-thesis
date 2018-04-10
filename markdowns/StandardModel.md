------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...

# Modern Cosmology & Large Scale Structure Formation

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
  ds^2 = -c^2dt^2 + a(t)^2 dl^2
  $$

  - where $a(t)$ represents the scale factor and the line segment $l$ describes the comoving distance independent of Hubble flow over any 3-dimensional coordinate space.

- Written in spherical coordinates, the FLRW metric takes the form

- $$
  ds^2 = -c^2dt^2 + R(t)^2 \left[  d\chi^2 + S_K(\chi)^2 \,  d\Omega^2   \right]
  $$

  - where $R(t)$ is the time-dependent radius of the Universe, $\chi$ is a dimensionless radial coordinate, and $d\Omega$ is the spherical coordinate space corresponding to $d\theta^2 + \sin^2 \! \theta \, d\phi^2$.

  - The radius $R(t)$ is related to the scale factor by $R(t) \equiv R_0 a(t)$ with a radius of curvature $R_0 = (\sqrt{|K|})^{-1}$ where $K$ is the curvature constant.  The physical comoving distance $d_c$ can be related to the dimensionless comoving coordinate $\chi$ by $d_c = R_0 \chi$. While, the 'true' distance $D$, otherwise known as the proper distance, depends on the scale factor and would be given by $D = a(t) \, d_c$. The geometry of the Universe $S_\kappa(\chi)$ depends on the curvature $K$ such that
    $$
    S_K(\chi) =
    \begin{cases}
    \sin^2 \! \chi & \text{if } \ K = +1 \hspace{5mm} \text{ (open `spherical' universe),}\\
    \chi & \text{if } \ K = 0 \hspace{9mm}  \text{ (flat universe)},\\
    \sinh^2 \! \chi & \text{if } \ K = -1 \hspace{5mm} \text{ (closed `hyperbolic' universe).}
    \end{cases}
    $$

  - Observations from the CMB amongst others strongly support a infinitely flat Universe such that $K \simeq 0$ and $R \to \infin$.

- While 

## Peculiar Velocity

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

The proportionality constant $H_0$ is better known as the Hubble constant, but is most usefully written as $H_0= 100\, h\,$\si{\km\per\s\per\Mpc} where $h$ is the dimensionless Hubble parameter defined by the current accepted value.



