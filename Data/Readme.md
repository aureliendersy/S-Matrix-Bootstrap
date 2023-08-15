In this Data Folder we have

1) Atkinson _Classical: Sets of points in the $z_1$ plane (separated in different regions) that lead to a set of ambiguous phase solutions. Details on the regions can be found [here](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.17.2492) or in our paper.

2) Atkinson_ML_Scans: Loss and $\sin \mu$ values obtained by training neural networks at different points in the $z_1$ plane. The networks are either initialized with a pretrained network at a fixed $z_1$ value (Fixed_Initialization), or with a pretrained network at a neighbouring $z_1$ value (Neighbour_Initialization).

3) Bootstrap: Errors on unitarity which comes by computing the unitarity equation in Mathematica at different $z$ points.

4) Finite_L_Class2: List of finite amplitude roots at $L=2$ (z1.csv and z2.csv) and $L=3$ (z1a/b, z2a/b, z3a/b) that correspond to ambiguous solutions where a single root is complex conjugated. At $L=3$, the amplitudes are class 2 (files a) or class 3 (files b).

5) Functions_Scans: Phases, $\sin \mu$'s and associated losses obtained by training neural networks on $B(z)=a z^2 + \epsilon$ at different $\epsilon$ values. Networks are trained using either the scaled or non-scaled unitarity loss.

6) Gradient_descent: Lists of visited points, gradients, losses and associated $\sin \mu$ values along two gradient descent trajectory. Traj 1 is for an ambiguous amplitude with a single conjugted root, whereas Traj 5 has two complex conjugated roots.

7) Polynomial_Scans: Losses and $\sin \mu$ values coming from training neural networks on families of moduli as $B(z) = az +b$ and $B(z)=cz^2+d$.





