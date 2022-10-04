# Quantum Mechanics

### Background to Quantum Mechanics
Quantum mechanics is the study of the physical properties of matter, on the scale of atomic or subatomic particles. 

Classical physics on the other hand studies matter and energy on a macroscopic scale - that is, on a scale that we are more used to seeing in daily life.


Though the mathematical basis of quantum mechanics is well-agreed upon (and verified through experiments), there exist many different ways to explain how these mathematical theories correspond to our experienced reality. These are known as **interpretations** of quantum mechanics, and there is no consensus on which one "best" represents our reality.

For this series of writeups, we will be explaining using the Copenhagen Interpretation. It is important to note, however, that Heisenberg's Uncertainty Principle still holds no matter which other interpretation is chosen. 


### Brief Introduction to the Copenhagen Interpretation
In day-to-day life, we are used to describing position with a definite value. If you see a football on the ground, you know the football is there. We say that the position of the football is at that point - exactly where we see it. And no matter how we kick the ball around, we know it will always have a position - it will always be somewhere we can describe with a real "location".

The same doesn't apply in quantum mechanics. Under the Copenhagen interpretation, observable quantities like position have no reality until they are measured. 

A state describes the conditions of a system. In each of these states, an observable quantity (e.g. position) can take on different values - imagine our ball being in various locations on a field. Until a measurement is performed, the system exists as a superposition of these quantum states.

This means the ball seems to be in multiple places at the same time, which is very unintuitive and suggests we need a different way to think about it. Since the ball doesn't always have a definite position where it can be found, we can only describe its location in terms of the probability of finding it in different locations. In other words, quantum theory can only provide us with a probability distribution for a measurement's outcome. 

Of course, if you can SEE the ball, you definitely know where it is. We know intuitively that the act of measurement must only give us one definite, actual value. How then does quantum mechanics explain this? 

This is known as the measurement problem, and the Copenhagen interpretation explains it as follows: When we perform a measurement on an observable quantity, we are forcing the system into a state where the observable has a single, definite value. This is known as an eigenstate of that observable.



As a (poorly contrived, but 100% original) analogy, think of a spinning coin. 

Is the coin showing heads or tails? While the coin is still spinning, this question has no meaning - if anything, it's showing neither.

But imagine now we slap the coin with our palm, flat onto the table. When we lift our hand up, we will see the coin necessarily shows either heads or tails. The act of measurement has forced it into an eigenstate, in which the observable value is either 'heads' or 'tails'. This is analogous to the wave-function collapse in the Copenhagen interpretation. When we measure a quantity, we suddenly force the system into any of the states that does have a definite value for that quantity. But while we aren't measuring it, the system can continue to exist as a superposition of these states, and the quantity returns to having no definite value.



### Heisenberg's Microscope
Heisenberg's microscope describes the thought experiment that Heisenberg formulated as an introduction to his uncertainty principle. Suppose we wish to determine the position and momentum of an electron, which we will (ironically) treat as a classical particle.

Let the wavelength of the light rays be $\lambda$.
Let the cone of light rays focusing on the electron make an angle $\varepsilon$ with the electron. 

The laws of classical optics tells us that we can only resolve the position of the electron to the following accuracy:
$$
\Delta{x}=\frac{\lambda}{\sin{\varepsilon}}
$$

We also know that when a photon strikes an electron, the electron experiences Compton recoil with momentum proportional to $\frac{h}{\lambda}$. But since the direction of the scattered photon can be anywhere within the cone of light rays, we can only determine the electron's momentum in the x direction to the following accuracy:
$$
\Delta{p}_{x} \approx \frac{h}{\lambda}\sin{\varepsilon}
$$

Suppose we want to decrease the uncertainty of the position, i.e. decrease $\Delta{x}$.

If we decrease the wavelength of light, we can resolve the position to a greater accuracy. But the photon will strike the electron with more momentum and result in even greater uncertainty in the electron's final momentum.

On the other hand, if we increase $\varepsilon$ by widening the microscope's aperture, we can also resolve the position to a greater accuracy (shown by the Rayleigh criterion). But since the angle the cone of light makes with the electron is larger, the scattered photon could be moving in a wider range of directions. This also increases the uncertainty in the electron's final momentum in the x-direction.

Looking at the equations together, we begin to get a picture of why we cannot perfectly determine both the momentum and the position of an electron. Any action taken to decrease the uncertainty of either momentum or position will increase the uncertainty in the other variable. 

Heisenberg used these results to formulate an approximate expression of the uncertainty principle,

$$
\Delta{x}\Delta{p_x} \approx \frac{\lambda}{\sin{\varepsilon}}
$$


### Confusion with the Observer Effect
Heisenberg's original thought experiment made use of the observer effect (also known as observer's paradox), in which the act of measurement causes the system to change. Unfortunately this has led to people incorrectly attributing the uncertainty principle TO the observer effect.

The observer effect is undeniably at play in the act of measurement, but its involvement is limited to the collapse of the wave function (at least, under the Copenhagen interpretation). The uncertainty in our measurements is not a result of the act of measurement introducing error to the system - rather, the uncertainty is instrinsic to all quantum systems. Even if we were to devise a measurement method that did not disturb the system by changing its momentum or position, Heisenberg's Uncertainty Principle would still hold because of the statistical uncertainty of those variables.


### So what does uncertainty mean?
Momentum and position are incompatible observables, and are special in that they are canonical conjugate quantities. That is, one is the Fourier transform of the other. Such pairs of variables do not commute, which implies that **no quantum state can simultaneously be a position eigenstate and a momentum eigenstate**. 

In other words, there exists no such preparation of a system such that only one possible value of BOTH position and momentum can be associated with it. If we measure the momentum and force the system into a momentum eigenstate, the state cannot be a position eigenstate - i.e. the value of momentum corresponds to multiple possible states, each with different values of position. There is a limit to how much we can know simultaneously about position and momentum, and this limit is quantified in Heisenberg's Uncertainty Principle.

<iframe width="420" height="315"  
src="https://www.youtube.com/embed/tgbNymZ7vqY">  
</iframe>