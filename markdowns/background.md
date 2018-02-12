#background
---
eqnos-cleveref: On
eqnos-plus-name: Eq.
...

## Doppler Effect

Suppose you are standing on the sidewalk and along the road a parked ambulance turns on its siren. As the ambulance siren blares, it approaches you and you notice that the pitch of the siren seems to have increased such that it sounds higher than it did previously. Then, as the ambulance passes and recedes behind you, another change occurs but now the pitch seems to have decreased such that it sounds much deeper than before. This is a classic example of the phenomenon known as the Doppler effect where a stationary observer experiences a change in frequency due to a moving wave source.  More precisely, the Doppler effect produces an observed shift in the original wave emitted such that an approaching wave source (i.e. the ambulance moving towards the observer) will seemingly appear to have an increase in frequency, meanwhile a receding wave source (i.e. the ambulance moving away from the observer) will appear to have a decrease in frequency. However, it is important to keep in mind that while a Doppler shift is observed, in actuality there are no changes to the emitted wave or the wave source itself. The relationship for the frequency observed by a stationary observer from a moving wave source is given by the expression:

$$
f_\text{obs} = f_\text{0} \left (\frac{v_\text{wave}}{v_\text{wave} \mp v_\text{source}}  \right ) 
$$
{#eq:classicdop}

where $f_\text{obs}$ describes the observed Doppler shifted frequency, $v_\text{wave}$ is the wave velocity, $v_\text{source}$ is the velocity of the moving wave source, and $f_\text{0}$ is the emitted frequency by the wave source\footnote{As you may have noticed, the relationship results in a constant Doppler shift in the frequency which is not what you would actually observe when an ambulance passes by. The increasing and decreasing in frequency is actually a product of the ambulance passing parallel to the observer which results in a changing angle between the moving wave source and the line of sight between the ambulance and the observer such that $v_{los} = v_\text{source} \cdot \text{cos}\ \theta$. However, if the ambulance were to drive directly at the observer, they would would hear a constant increase or decrease in the frequency as is the case in our example.}. The wave velocity $v_\text{wave}$ in the equation is the speed of the emitted wave and is defined by the wavelength $\lambda$ times the emitted frequency $f_0$ at which the wave oscillates (the wave speed of sound is approximately 343 $\si{m/s}$). The minus-plus sign in the denominator takes into account that the stationary observer would experience an increase in frequency when the wave source is moving towards them (i.e. minus sign) and a decrease in frequency when the wave source recedes away from them (i.e. plus sign). 

While in our ambulance example the Doppler shifted sound waves experienced by a stationary observer can accurately be described by @eq:classicdop, this form of the equation is only true for wave sources that move much slower than the speed of light. For electromagnetic waves (such as visible light) special relativity dictates that the relationship must be altered such that Lorentz symmetry\footnote{Lorentz symmetry states simply that the laws of physics must uphold in any reference frame.} is upheld. The relativistic form of the Doppler effect becomes
$$
\nu_{obs} = \nu_{0}\ \sqrt{\frac{1- \beta}{1 + \beta}}
$$
{#eq:reldop}

where $\nu$ is the relativistic notation for frequency (equivalent to $f$ in the classical case) and $\beta$ is the ratio of $v_\text{source}$ to the speed of light $c$. Note that $\beta$ is negative when the observer and the source are receding from each other and positive when the observer and the source are moving towards each other analogous to the minus-plus sign in the classical case. In the case that the speed of the wave source is much slower than the speed of the wave itself

**taylor expand for v << c gives rel --> classical**

For example, we can relate the speed at which light propagates $c$ to its frequency $f$ and wavelength $λ$ by the equation $c = f\ \lambda$. From this simple relation we can then see that @eq: dopfreq can be rewritten in terms of the wavelength of light such that:
$$
\lambda' = \left ( 1 \pm \frac{v_\text{source}}{c}  \right )  \lambda_\text{source}
$$
{#eq:doplambda}

where $\lambda'$ is the observed wavelength and $\lambda_\text{source}$ is the original wavelength emitted by the wave source.