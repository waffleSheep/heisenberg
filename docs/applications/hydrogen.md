# Determining the size of the hydrogen atom in the ground state


The total energy of the system is:

$$\begin{aligned}
E &= KE_{\text{electron}} + KE_{\text{proton}} + PE_{\text{electron-proton interaction}}\\
&= 0 + \frac{{p}^{2}}{2m} +\frac{(|e|)(-|e|)}{(4\pi{\epsilon}_{0}r)}
\end{aligned}
$$

where m = electron mass, and ${\epsilon}_{0} = \frac{{10}^{-9}}{36\pi} F/m$ also known as the permittivity of free space.

$$\begin{aligned}
E = 0 + \frac{{p}^{2}}{2m} -\frac{(|e|)(|e|)}{(4\pi{\epsilon}_{0}r)}
\end{aligned}
$$

The electron can be anywhere in the radius, r, of the atom at the ground state. hence the maximum uncertainty of the position of the electron in one dimension is r. From the Heisenberg Uncertainty Principle:

$$\begin{aligned}
\sigma_{x_x}\sigma_{p_x}&= \frac{h}{4\pi}\\
\end{aligned}
$$

Solving for the minimum uncertainty in momentum

$$\begin{aligned}
p(\sigma_{p_{min}}) \approx \frac{h}{4\sigma_{p_{xmax}}\pi}
\end{aligned}
$$

So,

$$\begin{aligned}
E &=  0 + \frac{{(\frac{\hbar}{2r})}^{2}}{2m} -\frac{(|e|)(|e|)}{(4\pi{\epsilon}_{0}r)}\\
&= \frac{{\hbar}^{2}}{8mr} -\frac{{|e|}^{2}}{(4\pi{\epsilon}_{0}r)}
\end{aligned}
$$

when $\frac{dE}{dr} = 0 at r = {r}_{1}$ , then that would be the lowest possible energy the atom would have, which would be at the ground state.

$$
\frac{d}{dr}(\frac{{h}^{2}}{8m{r}^{2}}-\frac{{|e|}^{2}}{4\pi{\epsilon}_{0}r})  = 0 \rightarrow - \frac{{h}^{2}}{4m{r}^{3}}+\frac{{|e|}^{2}}{4\pi{\epsilon}_{0}{r}^{2}} = 0\\
$$

$$
\begin{aligned}
\frac{{h}^{2}}{4mr}&=\frac{{|e|}^{2}}{4\pi{\epsilon}_{0}}\\
{r}_{1} &= \pi{\epsilon}_{0}\frac{{h}^{2}}{m{|e|}^{2}}\\
&= \pi \times \frac{{10}^{-9}}{36\pi} \times \frac{{(\frac{6.626x{10}^{-34}}{2\pi})}^{2}}{{(9.1 x {10}^{-31})(1.6 x {10}^{-19})}^{2}}\\
&= 1.33 x {10}^{-11}m\\
&= 0.0132Å
\end{aligned}
$$

Hence the radius of the hydrogen atom in the first ground state is $0.0132Å$.
