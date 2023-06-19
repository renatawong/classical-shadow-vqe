# Electronic structure problem (estimating ground state energy) with VQE and classical shadows
This notebooks implement the ideas of [1] and attempt to reconstruct the experimental results therein.

# Status
The notebooks are undergoing testing and debugging. 

# How to use
Requires the package predicting-quantum-properties from https://github.com/hsinyuan-huang/predicting-quantum-properties

There are four files that calculate the electronic structure problem:
1. [esp_rcs_vqe_qiskit.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/0c931801968c97d76ba769f921bdd6f396697823/esp_rcs_vqe_qiskit.ipynb) : Electronic structure problem using VQE with the vanilla classical shadow (i.e. randomised basis change).
2. [esp_rcs_vqe_qiskit_optimized.ipynb]() : As above but with optimization. 
3. [esp_dcs_vqe_qiskit.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/dec596a03eff866fccbf0d9505fac537b805d54e/esp_dcs_vqe_qiskit.ipynb) : Electronic structure problem using VQE with ``derandomised'' classical shadow (i.e. derandomised Hamiltonian used for basis change).
4. [esp_dcs_vqe_qiskit_optimized.ipynb](https://github.com/renatawong/classical-shadow-vqe/blob/cff1de7a79346f915471710eb395e3a7145c59bb/esp_dcs_vqe_qiskit_optimized.ipynb) : As above but with time optimization. 

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
