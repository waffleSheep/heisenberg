# Derivation of Heisenberg's Uncertainty Principle

To derive the principle, we need to find the variance for the position and momentum of a given particle.

As discussed earlier, the Schrodinger equation was empirically developed and was found to be

$$i\hbar {\frac {\partial }{\partial t}}\Psi (x,t)=\left[-{\frac {\hbar ^{2}}{2m}}{\frac {\partial ^{2}}{\partial x^{2}}}+V(x,t)\right]\Psi (x,t)$$

for a given quantum state $\Psi$. It was also discussed that the probability density amplitude function of the position of the particle in the sense that the probability of finding the particle between a and b is given by

$$\operatorname {P} [a\leq X\leq b]=\int _{a}^{b}|\Psi (x)|^{2}\,\mathrm {d} x.$$

Since the expectation for a variable is defined as such

$$\mu_x=\int _{-\infty}^{\infty}x\cdot\operatorname {P} [X=x]\,\mathrm {d} x$$

we find that that the expectation of position is

$$\mu_x=\int _{-\infty}^{\infty}x\cdot|\Psi (x)|^{2}\,\mathrm {d} x$$

and since the variance for a variable is defined as such

$$\sigma_x^2=\int _{-\infty}^{\infty}{(x-\mu_x)}^2\cdot\operatorname {P} [X=x]\,\mathrm {d} x$$

we find that the variance of position is

$$\sigma_x^2=\int _{-\infty}^{\infty}{(x-\mu_x)}^2\cdot|\Psi (x)|^{2}\,\mathrm {d} x.$$

Now, we must find the variance of momentum. However first we need to figure  out what the expectation of the momentum of the particle is. We will use the equation $p=mv$ to derive it

$$
\begin{aligned}
\mu_p&=m\frac{d\mu_x}{dt}\\
&=m\frac{d}{dt}\int _{-\infty}^{\infty}x\cdot|\Psi (x)|^{2}\,\mathrm {d} x\\
&=m\int _{-\infty}^{\infty}x\cdot \frac{\partial}{\partial t} \left (|\Psi (x)|^{2} \right)\,\mathrm {d} x
\end{aligned}
$$

Using schrodingers equation, we can derive the value for the inner term

$$
\begin{aligned}
\frac{\partial}{\partial t} \left (|\Psi|^{2} \right)
&=\frac{\partial}{\partial t} (\Psi^* \Psi)\\
&=\Psi^*\frac{\partial}{\partial t} ( \Psi)+\Psi\frac{\partial}{\partial t} ( \Psi^*) \\
&=\Psi^*{\frac {i\hbar}{2m}}{\frac {\partial ^{2}}{\partial x^{2}}}\Psi-\Psi{\frac {i\hbar}{2m}}{\frac {\partial ^{2}}{\partial x^{2}}} \Psi^*\\
&=\frac{i\hbar}{2m}\left(\Psi^*{\frac {\partial ^{2}}{\partial x^{2}}}\Psi-\Psi{\frac {\partial ^{2}}{\partial x^{2}}} \Psi^* \right)\\
&=\frac{i\hbar}{2m}\left(\Psi^*{\frac {\partial ^{2}}{\partial x^{2}}} \Psi+\frac {\partial \Psi}{\partial x}\frac {\partial \Psi^*}{\partial x}-\frac {\partial \Psi}{\partial x}\frac {\partial \Psi^*}{\partial x}-\Psi{\frac {\partial ^{2}}{\partial x^{2}}} \Psi\right)\\
&=\frac{i\hbar}{2m}\frac{\partial}{\partial x} \left (\Psi^*\frac{\partial \Psi}{\partial x}-\frac{\partial \Psi^*}{\partial x}\Psi \right)
\end{aligned}
$$

We can sub this back into the original equation

$$
\mu_p=\frac{i\hbar}{2}\int _{-\infty}^{\infty}x\cdot \frac{\partial}{\partial x} \left (\Psi^*\frac{\partial \Psi}{\partial x}-\frac{\partial \Psi^*}{\partial x}\Psi \right)\,\mathrm {d} x
$$

We can now do integration by parts

$$
\begin{aligned}
\mu_p&=\frac{i\hbar}{2}\left[x\left(\Psi^*\frac{\partial \Psi}{\partial x}-\frac{\partial \Psi^*}{\partial x}\Psi\right)\right]_{-\infty}^{\infty}-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}-\frac{\partial \Psi^*}{\partial x}\Psi\right)\,\mathrm {d} x\\
&=-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}-\frac{\partial \Psi^*}{\partial x}\Psi\right)\,\mathrm {d} x\\
&=-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}\right)\,\mathrm {d} x+\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\frac{\partial \Psi^*}{\partial x}\Psi\right)\,\mathrm {d} x
\end{aligned}
$$

We do integration by parts on the second term

$$
\begin{aligned}
\mu_p&=-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}\right)\,\mathrm {d} x+\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\frac{\partial \Psi^*}{\partial x}\Psi\right)\,\mathrm {d} x\\
&=-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}\right)\,\mathrm {d} x+[\Psi^*\Psi]_{-\infty}^{\infty}-\frac{i\hbar}{2}\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}\right)\,\mathrm {d} x\\
&=-i\hbar\int _{-\infty}^{\infty} \left(\Psi^*\frac{\partial \Psi}{\partial x}\right)\,\mathrm {d} x\\
&=\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x\\
\end{aligned}
$$

Viola, we have figured it out.


