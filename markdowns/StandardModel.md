------

eqnos-cleveref: On
eqnos-plus-name: Eq.
...

# Background: Standard Model of Cosmology 

- What is general relativity

- Using spacetime coordinates $(ct, x, y, z)$ to describe events.

  - where we define separation between two events by the line segment $ds^2 = -c^2 dt^2 + dx^2 + dy^2 + dz^2 \equiv \eta_{\mu\nu}dx^\mu dy^\nu​$, an invariant quantity under coordinate transformation\footnote{This means that from any inertial frame of reference, an observer would measure the same separation $ds​$.}

-  ​

  ### For next section on cosmology

  ​

$$
v_p \equiv \textbf{\textit{v}} \cdot \textbf{\hat{r}} = c \left ( \frac{z\text{obs} - z\text{cos}}{1 + z_\text{cos}}  \right)
$$

- $$
  1 + z = (1 + z_H)(1 + v_{pec}/c)
  $$

  ​

## Peculiar Velocity

Hubble's law represents an empirical relationship for the expanding universe where each galaxy is static with respect to cosmological expansion. Given @eq:Hubble we can estimate the cosmological redshift $z_\text{cos}$ due to expansion from $z_\text{cos} \equiv H_0 d/c$. However, an ideal Hubble's law neglects gravitational attraction to higher density regions of space which induce 'peculiar' motion that deviates from cosmological expansion velocity $H_0d$ (also known as the Hubble flow). The consequence of a continuous inflow of matter towards these regions of space is a state of over-density known as gravitational collapse, which provides the means for the formation and growth of structure in the local Universe. Thus, measurements of peculiar velocity are a compelling cosmological probe of local structure due to the motion of galaxies tracing the underlying density field. 

We can estimate peculiar velocities as deviations within the observed redshift $z_{obs}$ from Hubble's law as a result of Doppler redshift $z_\text{doppler}$ due to local motion. Unfortunately we are observationally limited to receding and approaching wavelengths along the 1D line-of-sight component of a galaxy's full 3D peculiar velocity vector. Any transverse motion along the line-of-sight is far too small to be detected through spectroscopic measurements and thus we would also expect any contribution to the line-of-sight to be in the form of noise in the signal. Following @eq:Hubble, at low-redshift where $v \ll c$, the line-of-sight component of the peculiar velocity $v_p$ is given by the familiar form

$$v_p \approx cz_\text{obs} - H_0d$$ {#eq:pecveloapprox}

\noindent where $c$ is the speed of light, $z_\text{obs}$ is the observed redshift, and $H_0d$ is the cosmological expansion velocity at a given comoving distance\footnote{Comoving distance refers to the real distance between two objects at rest with respect to the Hubble flow. In simpler terms, comoving distance is the physical distance between two objects in the absence of cosmic expansion.} $d$\footnote{Davis et al shows that due to redshift not being an additive property this crude approximation is only accurate for $z_\text{obs} << 0.1$, but for the introductory purposes of this section we find this form more than sufficient. We will revisit this equation in Section 2.#}. Therefore given a distance indicator, the comoving distance $d$ can be measured independently from the observed redshift $z_\text{obs}$ allowing us to estimate the peculiar velocity. The most common form of distance indicators are the various standard candles introduced in Sec 1.# which unfortunately suffer from large uncertainties. In contrast to the high accuracy redshift measurements available, the uncertainty on distance estimators can be upwards of $\simeq 20\%$ which can lead to uncertainties in the peculiar velocity measurement on the order of the velocity itself. Typical peculiar velocity measurement are expected to be of order \SI{300}{km/s} while the errors scale largely with the distance of the galaxy such that uncertainty $\delta_{v_p}$ can be approximated by $\delta_{v_p} \approx 0.20 H_0 d$. Given the large uncertainties, peculiar velocity measurements must be estimated through statistical means thus requiring large velocity surveys with both distance and redshift measurements\footnote{In Section 2.# we will discuss an estimator method developed by Watkins & Feldman that provides a more accurate method of statistically estimating peculiar velocities.}.