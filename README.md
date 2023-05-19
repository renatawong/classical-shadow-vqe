# Electronic structure problem (estimating ground state energy) with VQE and classical shadows
This notebooks implement the ideas of [1] and attempt to reconstruct the experimental results therein.

# Status
The notebooks are complete and undergoing testing. 

# How to use
Requires the package predicting-quantum-properties from https://github.com/hsinyuan-huang/predicting-quantum-properties

There are four files:
1. [esp_rcs.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/0c931801968c97d76ba769f921bdd6f396697823/esp_rcs.ipynb) : VQE using vanilla classical shadow.
2. [esp_rcs_optimized.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/f2902e2bb24a0c20e1144054e5a04d211a881613/esp_rcs_optimized.ipynb) : As above but with optimization. 
3. [esp_dcs.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/0c931801968c97d76ba769f921bdd6f396697823/esp_dcs.ipynb) : VQE using classical shadow with derandomized Hamiltonian.
4. [esp_dcs_optimized.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/e1fe074caf84d559fa279fb909f3c070ca9fe1be/esp_dcs_optimized.ipynb) : As above but with time optimization. 

Calculations using the optimized versions take significantly less time than with the non-optimised versions.

# Acknowledgements
The notebooks are based on the theory described in [1].

The code was written by Renata Wong (https://orcid.org/0000-0001-5468-0716).

This work benefited greatly from discussions with Prof. Hsi-Sheng Goan (National Taiwan University), Prof. Hao-Chung Cheng (National Taiwan University), Prof. Jyh-Pin Chou (National Changhua University of Education), and Hsin Yuan (Robert) Huang (California Institute of Technology). All remaining deficiencies are my own.

# References
[1] Hsin-Yuan Huang, Richard Kueng, and John Preskill, Efficient estimation of Pauli observables by derandomization, https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.030503

License
Apache License 2.0
