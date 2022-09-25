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

TBD TBD TBD HOW TF DO I FIND $\mu_{p^2}$

$$\mu_{p^2}=\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}\right]^2\Psi\right)\,\mathrm {d} x$$

Now that we know $\mu_{p^2}$ and $\mu_p$, we can find $\sigma_p^2$,

$$
\begin{aligned}
\sigma_p^2&=\mu_{p^2}-\mu_p^2\\
&=\mu_{p^2}-2\mu_p^2+\mu_p^2\\
&=\mu_{p^2}-2\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}\right]\mu_p\Psi\right)\,\mathrm {d} x+\mu_p^2\\
&=\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}-\mu_p\right]^2\Psi\right)\,\mathrm {d} x
\end{aligned}
$$

Now that we have both $\sigma_p^2$ and $\sigma_x^2$ we can solve with cauchy-schwarz inequality defined as such

$$
\begin{aligned}
\int _{-\infty}^{\infty}(f^*f)\,\mathrm {d} x\int _{-\infty}^{\infty}(g^*g)\,\mathrm {d} x \geq \int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d} x
\end{aligned}
$$

for values $f$ and $g$. Note also that

$$
\begin{aligned}
|z|^2 &= (Re(z))^2+(Im(z))^2\\
&\geq (Im(z))^2\\
&= \left(\frac{z-z^*}{2i} \right)^2
\end{aligned}
$$

Combining this, we see

$$
\int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d} x= \left(\frac{\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d}x-\int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x}{2i}\right)^2
$$

We can write the 2 equations in terms of $f$ and $g$ with the subs as such
$$
\begin{aligned}
f&=(x-\mu_x)\Psi\\
f^*&=\Psi^*(x-\mu_x)\\
g&=\left[-i\hbar\frac{\partial }{\partial x}-\mu_p\right]\Psi\\
g^*&=\Psi^*\left[-i\hbar\frac{\partial }{\partial x}-\mu_p\right]
\end{aligned}
$$

We now sub it in to the term in the previous inequality

$$
\begin{aligned}
\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d}x&= \int _{-\infty}^{\infty} \left(\Psi^*(x-\mu_x)\left[-i\hbar\frac{\partial }{\partial x}-\mu_p\right]\Psi\right)\,\mathrm {d} x\\
&=\int _{-\infty}^{\infty} \left(\Psi^*x\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x-\int _{-\infty}^{\infty} \left(\Psi^*x\mu_p\Psi\right)\,\mathrm {d} x\\
&-\int _{-\infty}^{\infty} \left(\Psi^*\mu_x\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x+\int _{-\infty}^{\infty} \left(\Psi^*\mu_x\mu_p\Psi\right)\,\mathrm {d} x\\
&=\int _{-\infty}^{\infty} \left(\Psi^*x\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x-\mu_x\mu_p-\mu_x\mu_p+\mu_x\mu_p\\
&=\int _{-\infty}^{\infty} \left(\Psi^*x\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x-\mu_x\mu_p
\end{aligned}
$$

Applying the same steps to conjugate, we get

$$
\int _{-\infty}^{\infty}(g^*f)\,\mathrm {d}x=\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}\right]x\Psi\right)\,\mathrm {d} x-\mu_x\mu_p
$$

If we compare them, we get

$$
\begin{aligned}
\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d}x-\int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x&=\int _{-\infty}^{\infty} \left(\Psi^*x\left[-i\hbar\frac{\partial }{\partial x}\right]\Psi\right)\,\mathrm {d} x\\
&-\int _{-\infty}^{\infty} \left(\Psi^*\left[-i\hbar\frac{\partial }{\partial x}\right]x\Psi\right)\,\mathrm {d} x\\
&=i\hbar \cdot \int _{-\infty }^{\infty }\Psi ^{*}\left[\left(-x\cdot {\frac {d\Psi}{dx}}\right)+{\frac {d(x\psi)}{dx}}\right]\,\mathrm {d} x\\
&=i\hbar \cdot \int _{-\infty }^{\infty }\Psi ^{*}\left[\left(-x\cdot {\frac {d\Psi}{dx}}\right)+\Psi+\left(x\cdot {\frac {d\Psi}{dx}}\right)\right]\,\mathrm{d}x\\
&=i\hbar\int _{-\infty }^{\infty }\Psi ^{*}\Psi \,\mathrm{d}x\\
&=i\hbar
\end{aligned}
$$

Finally, we can combine the inequality and what we found

$$
\begin{aligned}
\sigma_x^2\sigma_p^2 &=\int _{-\infty}^{\infty}(f^*f)\,\mathrm {d} x\int _{-\infty}^{\infty}(g^*g)\,\mathrm {d} x \\
&\geq \int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d} x\\
&=\left(\frac{\int _{-\infty}^{\infty}(f^*g)\,\mathrm {d}x-\int _{-\infty}^{\infty}(g^*f)\,\mathrm {d} x}{2i}\right)^2\\
&=\left(\frac{i\hbar}{2i}\right)^2\\
&=\left(\frac{\hbar}{2}\right)^2
\end{aligned}
$$

Square rooting this inequality, we get

$$
\sigma_x\sigma_p\geq\frac{\hbar}{2}
$$

Viola, we figured out