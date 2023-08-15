# S-Matrix-Bootstrap

Repository for hosting the analysis tools required for generating coherent amplitudes, satisfying the unitarity constraint.

### Overview and Motivation

The goal of this project is to place bounds on the phases on moduli appearing in 2 to 2 scalar scattering amplitudes. The amplitude has to respect unitarity, enforced by an integral 

$$B (z) \sin \phi (z) = \frac{1}{4 \pi} \int_{- 1}^1 d z_1  \int_0^{2 \pi} d
   \phi_1 B (z_1) B (z_2) e^{i \phi (z_1) - i \phi (z_2)} $$
   
   where we use $z_2 = zz_1 + (1 - z^2)^{1 / 2}  (1 - z_1^2)^{1 / 2} \cos \phi_1$. Here $B(z)$ represents the modulus, where $z$ is $\cos \theta$, with $\theta$ the scattering angle. The goal will be to solve this equation for a function $\phi(z)$, the phase, assuming that $B(z)$ is given.
   
##### ML angle

To tackle this problem we will represent $\phi(z)$ by a neural network and try and solve the integral equation, by characterizing it as a loss term $\mathcal{L}$. We will also implement a repulsive loss to characterize whether the solution is unique or not.

### Dependencies

We require 

- pytorch (1.12.1)
- numpy (1.23.2)
- tqdm (4.64.1)
- matplotlib (3.5.3)

### Files

The Notebooks can be executed directly. Where long runs are required to generate the data, we provide the option to either excecute the routine or load the data results from the Data tab
