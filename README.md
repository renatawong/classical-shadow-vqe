# Electronic structure problem (estimating ground state energy) with VQE and classical shadows
This notebooks implement the ideas of [1] and attempt to reconstruct the experimental results therein.

# Status
The notebooks are undergoing testing and debugging. 

# How to use
Requires the package predicting-quantum-properties from https://github.com/hsinyuan-huang/predicting-quantum-properties

There are five files that calculate the electronic structure problem:
1. [electronic_structure_problem_dcs.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/c2403b4b3940f6846cfceeae7e2d1f6102d3b0a9/electronic_structure_problem_dcs.ipynb) : Electronic structure problem with shadow (derandomized) applied on the optimal set of angles. This is the original idea in [1].
2. [vqe_rcs_qiskit.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/8e5f0060ceb3f4036c2b4508e1d02d168edae2f5/vqe_rcs_qiskit.ipynb) : Electronic structure problem using VQE with the vanilla classical shadow (i.e. randomised basis change).
3. [vqe_rcs_qiskit_optimized.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/16f33d1e10e0a91bdf09008d1daa390b7f95fd6a/vqe_rcs_qiskit_optimized.ipynb): As above but with optimization. 
4. [vqe_dcs_qiskit.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/403e615a20d58d6313b0bc858a3719b1793892a2/vqe_dcs_qiskit.ipynb) : Electronic structure problem using VQE with ``derandomised'' classical shadow (i.e. derandomised Hamiltonian used for basis change).
5. [vqe_dcs_qiskit_optimized.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/382d30f9ac8d1d8e2d1d6365aa4747cd57b2efae/vqe_dcs_qiskit_optimized.ipynb) : As above but with time optimization. 

Calculations using the optimized versions take significantly less time than with the non-optimised versions.

File [modified_derandomization.py](https://github.com/renatawong/classical-shadow-vqe/blob/6d5051170bc193637e8f8251ce8d80f027d3ea14/modified_derandomization.py) contains a modified version of the file 'data_acquisition_shadow.py' in the package 'predicting-quantum-properties' [2]. This modification allows the user to specify the number of derandomised operators to be generated. In the original version [2], the user had to specify the number of evaluations per observable, which did not allow for control over the total number of generated operators. 

# Acknowledgements
The notebooks are based on the theory described in [1].

The code was written by Renata Wong (https://renatawong.github.io/).

This work benefited greatly from discussions with Prof. Hsi-Sheng Goan (National Taiwan University), Prof. Hao-Chung Cheng (National Taiwan University), Prof. Jyh-Pin Chou (National Changhua University of Education), [Michał Stęchły](https://www.mustythoughts.com/about.html) (PsiQuantum), and Hsin Yuan (Robert) Huang (California Institute of Technology). All remaining deficiencies are my own.

# References
[1] Hsin-Yuan Huang, Richard Kueng, and John Preskill, Efficient estimation of Pauli observables by derandomization, https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.030503

[2] Hsin-Yuan Huang, Predicting quantum properties, https://github.com/hsinyuan-huang/predicting-quantum-properties

License
Apache License 2.0
