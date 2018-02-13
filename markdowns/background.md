# Background

---
eqnos-cleveref: On
eqnos-plus-name: Eq.
...

## Doppler Effect

Suppose you are standing on the sidewalk and along the road a parked ambulance turns on its siren. As the ambulance siren blares, it approaches you and you notice that the pitch of the siren seems to have increased such that it sounds higher than it did previously. Then, as the ambulance passes and recedes behind you, another change occurs but now the pitch seems to have decreased such that it sounds much deeper than before. This is a classic example of the phenomenon known as the _Doppler effect_ where a stationary observer experiences a change in frequency due to a moving wave source.  More precisely, the Doppler effect produces an observed shift in the original wave emitted such that an approaching wave source (i.e. the ambulance moving towards the observer) will seemingly appear to have an increase in frequency, meanwhile a receding wave source (i.e. the ambulance moving away from the observer) will appear to have a decrease in frequency. However, it is important to keep in mind that while a shift is observed, in actuality there are no changes to the emitted wave or the wave source itself. The relationship for the _Doppler shifted_ frequency observed is given by the expression:

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

where $\nu$ is the relativistic notation for frequency (equivalent to $f$ in the classical case) and $\beta$ is the dimensionless ratio $v/c$ of the relative velocity $v$ between the source and the observer ($ v = v_\text{source} - v_\text{rec}$) to the speed of light $c$. Note that $\beta$ is positive when the observer and the source are receding away from each other and negative when the observer and the source are approaching each other---analogous to $v_\text{source}$ in the classical case. The relativistic Doppler effect may seem quite different from our classical case in @eq:classicdop; however, if we Taylor expand about the low-velocity limit (for $v \ll c$) where the relative velocity is much slower than the speed of light we find that $\nu_\text{obs} = \nu_0 \left( 1 - \beta +  \mathcal{O}(\beta^2) \right) $. Using the same low-velocity analysis on @eq:classicaldop, we find that $f_\text{obs} = f_0 \left( 1 - \beta \right)$ such that the relativistic Doppler effect reduces to the classical case for relative velocities much less than the speed of light.

We will find it useful to define the relativistic Doppler shift in terms of the redshift $z$ of the initial signal as
$$
z \equiv \frac{\nu_{0}}{\nu_\text{obs}} - 1 = \frac{\Delta\nu}{\nu_\text{obs}} \equiv \frac{ \lambda_\text{obs}}{\lambda_0} - 1 =  \frac{\Delta\lambda}{\lambda_\text{0}}
$$
{#eq:redshift}

where we have used the wave velocity relation $c = \lambda \cdot \nu$ to write the redshift in terms of the equivalent wavelength and frequency relations. The term redshift is used because it implies that the signal's wavelength has been lengthened, synonymous to longer wavelengths in the visible spectrum corresponds to red light. Likewise, a negative redshift is equivalent to a blueshift, a shortening of the signal's wavelength. From the limiting case for the low-velocity regime where $v \ll c$, using our previous result in @eq:redshift we find that
$$
z \approx \beta = \frac{v}{c}
$$
where receding sources appear redshifted and approaching sources appear blueshifted relative to an observer.

## Standard Candles

- A Standard candle is a class of astronomical objects that possess an intrinsic quality shared amongst the class, a 'standard' so to speak, that provides a well known luminosity.

- Examples of standard candles include Cepheid variable stars, planetary nebula, Tully-Fisher relation for spiral galaxies, and supernovae amongst others.

- All of these contribute to the cosmic distance ladder, a chain of various methods used to measure different length scales. The foundation of the distance ladder is the geometric effect of measuring nearby astronomical objects called parallax. The parallax measures a distant object by measuring the apparent displacement as the observer changes their position and is described by $d = 1 / p$, where $d$ is the distance in parsecs and $p$ is the parallax angle in arcseconds. 

- By measuring the apparent brightness of an object and given the luminosity is known, we can define the inverse square law for light as
  $$
  \text{distance} = \sqrt{\frac{\text{luminosity}}{4 \pi \cdot (\text{apparent brightness})}}
  $$
  where $d$ is the distance, $L$ is the luminosity, and $b_\text{apparent}$ is the apparent brightness or the flux as measured on Earth of the object. From this equation, we can see that the accuracy of our distance measurements depends on how well we know the object's true luminosity. Thus, determining the most suitable and accurate standard candles is the trickiest aspect of distance measurements as each method introduces some form of uncertainty.

- Cepheid variables 

- Distance measurements provide the foundation for the structure and evolution of the universe---in other words, the _cosmology_ of our universe.

