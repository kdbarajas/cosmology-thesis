#background
---
eqnos-cleveref: On
eqnos-plus-name: Eq.
...

## Doppler Effect

Suppose you are standing on the sidewalk and along the road a parked ambulance turns on its siren. As the ambulance siren blares, it approaches you and you notice that the pitch of the siren seems to have increased such that it sounds higher than it did previously. Then, as the ambulance passes and recedes behind you, another change occurs but now the pitch seems to have decreased such that it sounds much deeper than before. This is a classic example of the phenomenon known as the Doppler effect where a stationary observer experiences a change in frequency due to a moving wave source.  More precisely, the Doppler effect produces an observed shift in the original wave emitted such that an approaching wave source (i.e. the ambulance moving towards the observer) will seemingly appear to have an increase in frequency, meanwhile a receding wave source (i.e. the ambulance moving away from the observer) will appear to have a decrease in frequency. However, it is important to keep in mind that while a Doppler shift is observed, in actuality there are no changes to the emitted wave or the wave source itself. The relationship for the Doppler shifted frequency observed by an observer is given by the expression:

$$
f_\text{obs} = f_\text{0} \left (\frac{v_\text{wave} + v_\text{rec}}{v_\text{wave} + v_\text{source}}  \right )
$$
{#eq:classicdop}

where $f_\text{obs}$ describes the observed Doppler shifted frequency, $v_\text{wave}$ is  the speed of the emitted wave and is defined by the wavelength $\lambda$ times the emitted frequency $f_0$ such that $v_\text{wave} = \lambda \cdot f_0$, $v_\text{rec}$ is the velocity of the receiver (i.e. the observer), $v_\text{source}$ is the velocity of the moving wave source, and $f_\text{0}$ is the emitted frequency by the wave source\footnote{As you may have noticed, the relationship results in a constant Doppler shift in the frequency which is not what you would actually observe when an ambulance passes by. The increasing and decreasing in frequency is actually a product of the ambulance passing parallel to the observer which results in a changing angle between the moving wave source and the line of sight between the ambulance and the observer such that $v_{los} = v_\text{source} \cdot \text{cos}\ \theta$. However, if the ambulance were to drive directly at the observer, they would would hear a constant increase or decrease in the frequency as is the case in our example.}. The minus-plus sign in the denominator takes into account that the stationary observer would experience an increase in frequency when the wave source is moving towards them (i.e. minus sign) and a decrease in frequency when the wave source recedes away from them (i.e. plus sign). We can see that this equation simplifies for our ambulance example where the observer is at rest such that $v_\text{rec} = 0$, $v_\text{source}$ is positive indicating the ambulance is moving towards the observer, and the wave being emitted is sound such that $v_\text{wave}$ is the speed of sound at approximately 343 $\si{m/s}$.

While in our ambulance example the Doppler shifted sound waves experienced by a stationary observer can accurately be described by @eq:classicdop, this form of the equation is only true for wave sources that move much slower than the speed of light. For electromagnetic waves (such as visible light) special relativity dictates that the relationship must be altered such that Lorentz symmetry\footnote{Lorentz symmetry states simply that the laws of physics must uphold in any reference frame.} is upheld. The relativistic form of the Doppler effect becomes
$$
\nu_\text{obs} = \nu_{0}\ \sqrt{\frac{1- \beta}{1 + \beta}}
$$
{#eq:reldop}

where $\nu$ is the relativistic notation for frequency (equivalent to $f$ in the classical case) and $\beta$ is the ratio $v/c$ of the relative velocity $v$ between the source and the observer to the speed of light $c$. Note that $\beta$ is negative when the observer and the source are receding from each other and positive when the observer and the source are moving towards each other analogous to the minus-plus sign in the classical case. By taking the low-velocity limit of @eq:reldop, for $v \ll c$ we find that $\nu_\text{obs} = \nu_0 \left( 1 - \beta +  \mathcal{O}(\beta^2) \right) $ using our previous notation. Using the same low-velocity limit analysis on @eq:classicaldop, we find that $f_\text{obs} = f_0 \left( 1 - \beta +  \mathcal{O}(\beta^2) \right)$ 

It is often useful to define the relativistic Doppler shift in terms of the redshift $z$ of the initial signal as
$$
z \equiv \frac{\nu_{0}}{\nu_\text{obs}} - 1 = \frac{\Delta\nu}{\nu_\text{obs}} \equiv \frac{ \lambda_\text{obs}}{\lambda_0} - 1 =  \frac{\Delta\lambda}{\lambda_\text{0}}
$$
{#eq:redshift}

where we have used the wave velocity relation $c = \lambda \cdot \nu$ to write the redshift in terms of the wavelength and frequency. The term redshift is used because a redshifted signal implies that t

%$\Delta \nu$ is the difference between the emitted and observed frequency $\nu_0$ and $\nu_\text{obs}$, $\Delta \lambda$ is the difference between the observed and emitted wavelength $\lambda_\text{obs}$ and $\lambda_0$, and 



The relativistic Doppler effect may seem quite different from our classical case in @eq:classicdop, however if we take the limit that the relative velocity is much slower than the speed of light

**taylor expand for v << c gives rel --> classical**
