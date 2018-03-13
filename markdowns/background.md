# Background

---
eqnos-cleveref: On
eqnos-plus-name: Eq.
...

## Doppler Effect

Suppose you are standing on the sidewalk and along the road a parked ambulance turns on its siren. As the ambulance siren blares, it approaches you and you notice that the pitch of the siren seems to have increased such that it sounds higher than it did previously. Then, as the ambulance passes and recedes behind you another change occurs, but now the pitch seems to have decreased such that it sounds much deeper than before. This is a classic example of the phenomenon known as the _Doppler effect_ where a stationary observer experiences a change in frequency due to a moving wave source.  More precisely, the Doppler effect produces an observed shift in the original wave emitted such that an approaching wave source (i.e. the ambulance moving towards the observer) will seemingly appear to have an increase in frequency, meanwhile a receding wave source (i.e. the ambulance moving away from the observer) will appear to have a decrease in frequency. However, it is important to keep in mind that while a shift is observed, in actuality there are no changes to the emitted wave or the wave source itself. The relationship for the _Doppler shifted_ frequency observed is given by the expression:
$$
f_\text{obs} = f_\text{0} \left (\frac{v_\text{wave} + v_\text{receiver}}{v_\text{wave} + v_\text{source}}  \right )
$$
{#eq:classicdop}

where $f_\text{obs}$ describes the observed Doppler shifted frequency, $v_\text{wave}$ is  the speed of the emitted wave and is defined by the wavelength $\lambda$ times the emitted frequency $f_0$, $v_\text{receiver}$ is the velocity of the observer receiving the signal (positive when moving towards the source and negative in the opposite direction), $v_\text{source}$ is the velocity of the moving wave source emitting the signal (positive when receding from the observer and negative in the opposite direction), and $f_\text{0}$ is the emitted frequency by the wave source\footnote{As you may have noticed, the relationship results in a constant Doppler shift in the frequency which is not what you would actually observe when an ambulance passes by. The increasing and decreasing in frequency is actually a product of the ambulance passing parallel to the observer which results in a changing angle between the moving wave source and the line of sight between the ambulance and the observer such that $v_{_{LOS}} = v_\text{source} \cdot \text{cos}\ \theta$. However, if the ambulance were to drive directly at the observer, they would would hear a constant increase or decrease in the frequency as is the case in our example.}. We can see that this equation simplifies for our ambulance example where the observer is at rest such that $v_\text{receiver} = 0$, $v_\text{source}$ is negative indicating the ambulance is moving towards the observer, and $v_\text{wave}$ is the speed of sound at approximately 343 $\si{m/s}$. Given these conditions, we can write the Doppler effect for sound observed by a stationary observer (as in our ambulance example) as
$$
f_\text{obs} = f_\text{0} \left (\frac{1}{1 -\alpha}  \right )
$$
{#eq:ambdop}

where we have simplified the equation in terms of the dimensionless $\alpha$ velocity term equivalent to $v_\text{source} / v_\text{wave}$, the ratio of the source velocity to the speed of the wave.

While the Doppler shifted sound waves experienced by an observer can accurately be described by @eq:classicdop and @eq:ambdop, this form of the equation is only true for wave sources that move much slower than the speed of light. For electromagnetic waves (such as visible light) special relativity dictates that the relationship must be altered such that Lorentz symmetry\footnote{Lorentz symmetry states simply that the laws of physics must uphold in any reference frame.} is upheld. Therefore, the relativistic form of the Doppler effect becomes
$$
\nu_\text{obs} = \nu_{0}\ \sqrt{\frac{1- \beta}{1 + \beta}}
$$
{#eq:reldop}

where $\nu$ is the relativistic notation for frequency (equivalent to $f$ in the classical case) and the dimensionless $\beta = v/c$ is ratio between the relative velocity $ v = v_\text{source} - v_\text{rec}$ to the speed of light $c$. Note that $\beta$ is positive when the observer and the source are receding away from each other and negative when the observer and the source are approaching each other---analogous to $v_\text{source}$ in the classical case. The relativistic Doppler effect may seem quite different from our classical case in @eq:classicdop; however, if we Taylor expand about the low-velocity limit (for $v \ll c$) where the relative velocity is much slower than the speed of light we find that $\nu_\text{obs} = \nu_0 \left( 1 - \beta +  \mathcal{O}(\beta^2) \right) $. Using the same low-velocity analysis on @eq:classicaldop, we find that $f_\text{obs} = f_0 \left( 1 - \beta \right)$ such that the relativistic Doppler effect reduces to the classical case for relative velocities much less than the speed of light.

We will find it useful to define the relativistic Doppler shift in terms of the redshift $z$ of the initial signal as
$$
z \equiv \frac{ \lambda_\text{obs}}{\lambda_\text{em}} - 1 =  \frac{\Delta\lambda}{\lambda_\text{em}} = \sqrt{\frac{1 + \beta}{1-\beta}} - 1
$$
{#eq:redshift} %z \equiv \frac{\nu_{0}}{\nu_\text{obs}} - 1 = \frac{\Delta\nu}{\nu_\text{obs}} \equiv \frac{ \lambda_\text{obs}}{\lambda_0} - 1 =  \frac{\Delta\lambda}{\lambda_\text{0}}

where we have used the wave velocity relation $c = \lambda \cdot \nu$ to write the redshift in terms of wavelength. The term redshift is used because it implies that the signal's wavelength has been lengthened, synonymous to longer wavelengths in the visible spectrum corresponds to red light. Likewise, a negative redshift is equivalent to a blueshift, a shortening of the signal's wavelength. From the limiting case for the low-velocity regime where $v \ll c$, using our previous result in @eq:redshift we find that
$$
z \simeq \frac{v}{c}
$$


{#eq:lowvelocity}

where receding sources appear redshifted and approaching sources appear blueshifted relative to an observer.

## Standard Candles

- A Standard candle is a class of astronomical objects that possess an intrinsic quality shared amongst the class, a 'standard' so to speak, that provides a well known luminosity.

- Examples of standard candles include Cepheid variable stars, planetary nebula, Tully-Fisher relation for spiral galaxies, and supernovae amongst others.

- All of these contribute to the cosmic distance ladder, a chain of various techniques used to measure different length scales. The foundation of the distance ladder is the geometric effect of measuring nearby astronomical objects called parallax. The parallax uses the apparent displacement of a distant object as the observer changes their position to measure the distance and is described by $d = 1 / p$ (for $p \ll 1\, \text{radian}$), where $d$ is the distance in parsecs and $p$ is the parallax angle in arcseconds. While this method provides some of the most accurate distance measurements, it is limited by the apparent displacement which for large distances becomes difficult to resolve\footnote{Parallax measurements from ground-based telescopes are able to resolve to distances of about 50-100 \si{\parsec}, while space-based telescopes are able to extend this limitation to 200-300 \si{\parsec} within 10% accuracy.}.

- Despite the limitations of the parallax, the accuracy of the method allows astronomers to calibrate other methods that can measure distances at much greater length scales on the cosmic distance ladder. Cepheid variables are stars that undergo a period of pulsation---a defined period of contraction and expansion---during which a change in brightness is observed\footnote{It should be noted that when we mention brightness we are explicitly referring to the flux of light we measure in \si{\W\per\metre\squared}.}. Due to the change in physical size, the absolute brightness or _luminosity_ of the Cepheid changes such that we observe a change in apparent brightness on Earth. What makes Cepheid variables an important standard candle is that not only does this intrinsic quality holds amongst the class, but more importantly, from empirical evidence we know that there is a direct relationship between the period of pulsation and the true luminosity of Cepheids: unsurprisingly, we call this the _period--luminosity relationship_. Distance measurements are normally a challenge to calculate due to the required luminosity as defined by the inverse square law for light:
  $$
  \text{apparent brightness} = \frac{\text{Luminosity}}{4 \pi \cdot d^2}
  $$
  {#eq:invsqrlaw}

  where $d$ is the distance, $L$ is the luminosity, and $B$ is the apparent brightness as measured on Earth. But, by measuring the period of pulsation from changes in apparent brightness we are able to determine the luminosity and thus measure distance to Cepheids in galaxies far greater than the reach of parallax measurements. The accuracy of the period--luminosity relationship is dependent, however, on standard luminosity measurement to nearby Cepheids in which the parallax distance can be used to calibrate the method. For example, in 2002 the Hubble Space Telescope in partnership with the Hipparchus Satellite was able to use the parallax method to determine the most accurate distance measurement to the closest known Cepheid variable star, Delta Cephei, thus establishing a cosmic benchmark on the ladder for other distance methods. The period--luminosity relationship is often regarded as the stepping stone by which other methods are compared against to improve the accuracy of our distance measurements.

- A more common astronomical method of measuring distance analogous to the inverse square law of light in @eq:invsqrlaw involves the magnitude system, a logarithmic magnitude scale of a stellar object's brightness\footnote{invented by the Greek astronomer Hipparchus and Ptolemy. Eye sees logarithmically. Makes sense!}. Due to the logarithmic nature, the system is fairly counterintuitive such that an object brightness are given in 'reverse order' whereby brighter objects have a negative magnitude while dimmer objects have a positive magnitude. We define the apparent magnitude (as seen from Earth) as
  $$
  m \equiv m_a - m_b = -2.5 \log_{10} \left( \frac{B_a}{B_b} \right)
  $$
  {#eq:mag}

  From @eq:mag it is clear that a change of 1 magnitude corresponds to a 2.5 decrease in brightness between the objects. In order to standardize the relative comparison of magnitudes we compare stellar objects to the relative brightness to Vega such that objects that are brighter have a negative magnitude and objects that are dimmer have a positive magnitude\footnote{By this standard, it would naturally follow that Vega has a reference magnitude of 0}. Just as in @eq:invsqrlaw, in order to know the absolute magnitude we need to know the distance to the stellar object and we define this relationship as
  $$
  M = m - 2.5 \log_{10} \left[ \left( \frac{d}{10 \si{\parsec}} \right)^2 \right] \
  $$
  {#eq:absmag}

  The convention used here is to calculate the absolute magnitude as would be seen from 10\si{\parsec} away for all objects to standardize the method. If we simplify the equation we can rewrite @eq:absmag in terms of what we call the _distance modulus equation_ such that
  $$
  m - M = -5 + 5  \log_{10} (d)
  $$
  {#eq:distmod}

- Building off the stepping stone of the Cepheid' period--luminosity relationship, we can use the Tully-Fisher relation and Fundamental plane to extend the distance ladder to scales on the order of 1\si{\Gigaparsec}---the length scales of galaxy clusters. The Tully-Fisher relation is an empirically driven relationship between the rotational velocity of a galaxy and its absolute magnitude. In the context of the distance ladder it forms one of the most important distance estimators due to its measurement of the 21-centimeter hydrogen line, a far infrared line in the microwave spectrum, which is relatively unperturbed by objects that normally are opaque to shorter wavelengths\footnote{This technique is especially important to physical cosmology for its accurate prediction of the ratio of luminous matter in the galaxy disk to the dark matter halo that surrounds it. For further reading refer to Desmond et al., 2015 on the Tully-Fisher Relation and mass-size relations to halo abundance. https://arxiv.org/abs/1506.00169}. Given the 21-centimeter hydrogen line, we can measure the redshift and blueshift due to the rotation of a galaxy and estimate the rotational velocity of the galaxy. However, given that we need distance estimates to measure the luminosity in terms of the absolute magnitude, again we can see the distance ladder in effect in that we use Cepheid distance measurements from both parallax and period-luminosity relationship within individual galaxies to calibrate the distance to the galaxy themselves. Subsequently, we can plot the rotational velocity and the absolute magnitude of individually calibrated galaxies to show the Tully-Fisher relation. Thus, given a rotational velocity from far redshift objects we can not only estimate the absolute magnitude, but more importantly a distance estimate that otherwise wouldn't be possible.

- As we have seen, these techniques often overlap in the length scales they measure which is important for the calibration of the ladder through overlapping distance measurement within individual galaxies allowing allowing for multiple classes of distance estimators. Moreover, from @eq:invsqrlaw equation, we can see that the accuracy of our distance estimates depends on how well we know the object's true luminosity is known. Thus, determining the most suitable and accurate standard candles is the trickiest aspect of distance measurements as each method introduces some form of uncertainty. Regardless of the challenges in the method, distance measurements are one of the only methods that allow us to probe the cosmos and test our theories of the Universe. From this perspective, we see that distance measurement truly provide the foundation for understanding the structure and evolution of the universe---the _cosmology_ of our universe.

## Hubble's Law

- In the late 1920s using distance and redshift measurements, Edwin Hubble found that a galaxy's relative velocity away from Earth is proportional to the distance between us. The relationship now known as Hubble's law can be expressed as 

- $$
  v \simeq cz = H_0 d
  $$

  {#eq:Hubble}

  where we have expressed the relative velocity $v$ (in \si{km\per\s}) in terms of the low-velocity limit from @eq:lowvelocity, $H_0$ is the constant of proportionality known as the Hubble constant in \si{\km\per\s\per\Mpc}, and $d$ is the galaxy's distance in \si{Mpc}.

- While the redshift observed on Earth is often interpreted as a Doppler shift due to the method of measurement, this leads to a troubling interpretation of the Universe. That being that if the relative velocity is due to a Doppler redshift, than this would imply that everything in the night sky is receding away from us and that the Earth is located in a privileged place in the Universe. However, as Hubble amongst others had noticed, this statement is in obvious conflict with the Copernican principle which states that humans are not privileged observers of the Cosmos--i.e. that we are not located anywhere special with regards to the Universe around us. Another possible interpretation that does not require sacrificing the Copernican principle had been proposed independently as part of solutions to Einstein's field equation for general relativity by the Soviet mathematician Alexander Friedmann and the French astronomer Georges Lamaitre: that we reside in an expanding universe and Hubble's law provided the first empirical evidence supporting this theory. Under this interpretation, the relative velocity is not a result of intrinsic motion of galaxies away from us, but rather the result of the space between us stretching.

- Moreover, Hubble's law not only implies that the Universe is expanding, but that it is doing so at an accelerating rate. The Hubble constant is currently measured in the range of 67-75 \si{\km\per\s\per\Mpc}\footnote{Add footnote on discrepancies between Planck Satellite and Supernovae Type Ia measurements}, meaning that every megaparsec of space is being stretched at a rate of approximately 70 \si{km\per\s}.


​

![img](https://www.astro.rug.nl/~weygaert/tim1publicpic/dtfe/2dFpanel.dtfe.lres.gif)