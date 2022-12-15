# S-Matrix-Bootstrap

Repository for hosting the analysis tools required for solving the phase shift integral equation.

### Overview and Motivation

The goal of this project is to place bounds on the phase shift appearing in 2 to 2 scalar scattering amplitudes. The phase shift can be determined by an integral 

$$B (z) \sin \phi (z) = \frac{1}{4 \pi} \int_{- 1}^1 d z_1  \int_0^{2 \pi} d
   \phi_1 B (z_1) B (z_2) e^{i \phi (z_1) - i \phi (z_2)} $$
   
   where we use $z_2 = zz_1 + (1 - z^2)^{1 / 2}  (1 - z_1^2)^{1 / 2} \cos \phi_1$. Here $B(z)$ represents the differential cross section, where $z$ is $\cos \theta$, with $\theta$ the scattering angle. The goal will be to solve this equation for a function $\phi(z)$, the phase shift, assuming that $B(z)$ is given.
   
##### ML angle

To tackle this problem we will represent $\phi(z)$ by a neural network and try and solve the integral equation, by characterizing it as a loss term $\mathcal{L}$.
