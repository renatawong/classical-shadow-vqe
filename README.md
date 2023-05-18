# Estimating ground state energy with classical shadows
This notebook implements the ideas of [1] and attempts to reconstruct the experimental results therein.

# Status
This notebook is now complete and undergoing testing. 

# How to use
Requires the package predicting-quantum-properties from https://github.com/hsinyuan-huang/predicting-quantum-properties

There are three files:
1. Electronic_structure_problem_vqe_randomized_classical_shadow.ipynb: VQE using vanilla classical shadow.
2. Electronic_structure_problem_vqe_derandomized_classical_shadow.ipynb: VQE using classical shadow with derandomized Hamiltonian.
3. Electronic_structure_problem_vqe_derand_classical_shadow_optimized.ipynb: As above but with time optimization. The calculation takes significantly less time than the non-optimised version (2).

# Acknowledgements
This notebook is based on the theory described in [1].

The code was written by Renata Wong (https://orcid.org/0000-0001-5468-0716).

This work benefited greatly from discussions with Prof. Hsi-Sheng Goan (National Taiwan University), Prof. Hao-Chung Cheng (National Taiwan University), Prof. Jyh-Pin Chou (National Changhua University of Education), and Hsin Yuan (Robert) Huang (California Institute of Technology). All remaining deficiencies are my own.

# References
[1] Hsin-Yuan Huang, Richard Kueng, and John Preskill, Efficient estimation of Pauli observables by derandomization, https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.030503

License
Apache License 2.0
