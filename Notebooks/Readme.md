Here we provide 4 notebooks for reproducing the plots of our paper. 
When generating the data takes too long (e.g for a scanning run best done on the cluster) we provide the option to directly load the data that is present in the Data folders.

The notebooks are

1) 2to2_Scattering_Partial_waves: Plotting the ambiguous $L=2,3$ finite partial wave solutions that have only one complex conjugated root.
2) 2to2_Scattering_Phase_Recovery: Given an input modulus $B(z)$ we train a network to recover $\phi(z)$ consistent with unitarity. We also perform scanning runs over polynomial $B(z)$ to survey which ones can lead to valid unitary amplitudes. We also recover the Crichton ambiguity phase solutions by adding a repulsive loss
3) 2to2_Scattering_Atkinson_Ambiguities: Given a specific parameterization of the amplitude by complex conjugating a single root $z_1$ we can recover ambiguous solutions. We survey the $z_1$ plane to identify potential solutions and compare it to the original results. We also do gradient descent in that space to find a solution with the lowest $\sin \mu$ value. We reeiterate the exercise by complex conjugating two roots and showing that we can still recover ambiguous unitary phase solutions.
4) 2to2_Scattering_bootstrap: Given a pair of $B(z)$ that come from the bootstrap program where elastic unitarity is emerging, we try to recover the appropriate phase with our neutal networks. We also characterize the resulting deviation from unitarity.
