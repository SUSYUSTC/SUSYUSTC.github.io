---
layout: archive
title: "Research"
permalink: /research/
excerpt: "Research"
author_profile: true
---

<h3> Quantum-classical hybrid quantum algorithms </h3>

Quantum computing is heralded as a groundbreaking approach for simulating physical and chemical systems. Among the techniques available, the Variational Quantum Eigensolver (VQE) algorithm is particularly prominent in the current noisy intermediate-scale quantum (NISQ) era, marked by a limited number of qubits and relatively high error rates. The stabilizer formalism stands out as a powerful mechanism for enhancing the efficacy of the VQE algorithm. This formalism can be utilized through both the Schrödinger and Heisenberg pictures to improve quantum simulations.

In the Schrödinger picture, we can prepare stabilizer states as the initial configurations for quantum circuits. Meanwhile, in the Heisenberg picture, the Hamiltonian can be classically transformed using Clifford operations, a process that retains the eigenvalues of the Hamiltonian unchanged. Our research has led to the development of algorithms that optimize VQE performance for different system types using these pictures. For chemical systems, where mean-field theory provides a qualitative foundation, we develop the Clifford-based Hamiltonian engineering for molecules (CHEM) algorith. With an arbitrary hardware-efficient ansatz as input, this method effectively generates the Hartree-Fock state as the initial state, and also maximizes the initial energy gradients. In the realm of strongly-correlated systems, our efforts are geared towards creating scalable algorithms to identify exact stabilizer ground states, which can then be used as the starting point for VQE. Especially, a linear-scaled algorithm is developed to obtain the exact stabilizer ground states of 1D local Hamiltonians.

Beyond its role in boosting the performance of the Variational Quantum Eigensolver (VQE), the stabilizer formalism offers a foundational approach for the development of sophisticated quantum state ansätze capable of describing complex quantum systems. Drawing an analogy to the Hartree-Fock state, which serves as the cornerstone for developing theories like Møller-Plesset perturbation and coupled cluster theories, stabilizer ground states similarly provide a robust starting point. This opens up new avenues for constructing advanced quantum state ansatz, thereby extending our ability to describe and understand the intricate behaviors of quantum systems with greater precision.


References:

[1] **Sun, J.**, Cheng, L. & Li, W. (2024). Towards chemical accuracy with shallow quantum circuits: A Clifford-based Hamiltonian engineering approach. Journal of Chemical Theory and Computation. [[link](https://pubs.acs.org/doi/10.1021/acs.jctc.3c00886)]

[2] **Sun, J.**, Cheng, L. & Zhang, S.-X. (2024). Stabilizer ground states: theory, algorithms and applications. arXiv preprint arXiv:2403.08441. [[link](https://arxiv.org/abs/2403.08441)]

<h3> Molecular orbital based machine learning (MOB-ML) </h3>

Chemistry fundamentally revolves around the interactions of atoms and electrons, a complex dance orchestrated by the rules of quantum mechanics. Quantum chemistry, drawing from these principles, provides tools for calculating molecular properties, yet achieving desired accuracy for medium to large molecules remains a computational challenge. To bridge this gap, we introduced Molecular-Orbital-Based Machine Learning (MOB-ML), a novel approach that extracts highly accurate molecular property predictions akin to those obtained from sophisticated wavefunction theory, but at the significantly lower computational cost associated with the Hartree-Fock method.

MOB-ML is meticulously engineered to adhere to the core physical principles underlying reliable quantum chemistry theories. These include translational and rotational invariance, the permutation symmetries of atoms and orbitals, and size consistency. The model also respects equivariance relations, enabling it to generalize across tensorial and response properties with the same level of precision observed for scalar properties. This robust framework allows MOB-ML to accurately address a wide range of chemical phenomena, including organic molecules, intermolecular forces, transition states, and open-shell systems.

Further enhancing its utility, MOB-ML incorporates cutting-edge machine learning algorithms, such as alternative black-box matrix multiplication (AltBBMM) and kernel addition Gaussian process regression (KA-GPR). These innovations significantly improve the efficiency of machine learning applications without compromising accuracy. With these advancements, MOB-ML has demonstrated superior performance in comparison to other contemporary quantum machine learning methodologies globally, and it has been successfully applied in creating highly accurate potential energy surfaces (PES) for practical use.

References:

[1] Husch, T., **Sun, J.**, Cheng, L., Lee, S. J., & Miller III, T. F. (2021). Improved accuracy and transferability of molecular-orbital-based machine learning: Organics, transition-metal complexes, non-covalent interactions, and transition states. _The Journal of Chemical Physics_, 154, 064108.

[2] **Sun, J.**, Cheng, L., & Miller III, T. F. (2021). Molecular Energy Learning Using Alternative Blackbox Matrix-Matrix Multiplication Algorithm for Exact Gaussian Process. _NeurIPS 2021 AI for Science Workshop_.

[3] Cheng, L., **Sun, J.** & Miller III, T.F. (2022). Accurate Molecular-Orbital-Based Machine Learning Energies via Unsupervised Clustering of Chemical Space. _Journal of Chemical Theory and Computation_, 18, 8, 4826–4835.

[4] **Sun, J.**, Cheng, L., & Miller III, T. F. (2022). Molecular Dipole Moment Learning via Rotationally Equivariant Gaussian Process Regression with Derivatives in Molecular-orbital-based Machine Learning. _The Journal of Chemical Physics_, 157, 104109.

[5] Cheng, L., **Sun, J.**, Emiliano Deustua, J., Bhethanabotla, V. C., & Miller III, T. F. (2022). Molecular-orbital-based Machine Learning for Open-shell and Multi-reference Systems with Kernel Addition Gaussian Process Regression. _The Journal of Chemical Physics_, 157, 154105.

[6] Lu, F., Cheng, L., DiRisio, R.J., Finney, J.M., Boyer, M.A., Moonkaen, P., **Sun, J.**, Lee, S.J., Deustua, J.E., Miller III, T.F. and McCoy, A.B. (2022). Fast near ab initio potential energy surfaces using machine learning. _The Journal of Physical Chemistry A_, 126(25), 4013-4024.

<h3> Ring-polymer molecular dynamics (RPMD) </h3>

Classical molecular dynamics methods excel in simulating large chemical and biological systems but struggle to capture the nuclear quantum effects crucial for light atoms like hydrogen. To tackle this, we turned to Ring-Polymer Molecular Dynamics (RPMD), a technique that approximates these quantum effects in a semi-classical way.

In our latest study, we unveiled a new class of RPMD integrators, focusing on their accuracy, speed of convergence, stability, and their ability to work regardless of the system's size. Notably, the "BCOCB" type integrator emerged as the top performer. We used this integrator to accurately calculate reaction rates for the OH+CH4 reaction, achieving results that closely match experimental data. This work highlights the potential of RPMD, especially with our integrators, in making quantum simulations more accurate and broadly applicable.

References:

[1] Rosa-Raíces, J. L.<sup>\*</sup>, **Sun, J.**<sup>\*</sup>, Bou-Rabee, N., & Miller III, T. F. (2021). A generalized class of strongly stable and dimension-free T-RPMD integrators. _The Journal of chemical physics_, 154, 024106.

[2] Gui, X., Fan, W., **Sun, J.**, & Li, Y. (2022). New Stable and Fast Ring-Polymer Molecular Dynamics for Calculating Bimolecular Rate Coefficients with Example of OH+CH<sub>4</sub>. _Journal of Chemical Theory and Computation_, 18, 9, 5203–5212.

<h3> Electron transport in semiconductors </h3>

The study of electron transport under high electric fields is both fundamentally intriguing and practically crucial for semiconductor technology. A comprehensive theoretical understanding of electron transport necessitates precise calculations of electron-phonon interactions. Yet, the complexity and high computational demands often lead to the simplification of these calculations by omitting multi-phonon processes, which are critical for accuracy.

In our recent research, we delved into the high-field transport characteristics of Gallium Arsenide (GaAs), specifically incorporating the effects of two-phonon scattering processes. This inclusion sheds light on and resolves a longstanding debate concerning the intensity of intervalley scattering in GaAs, a discrepancy previously noted between transport and optical studies. Our findings not only enhance the accuracy of electron transport models but also provide a more coherent understanding of electron-phonon interactions in semiconductors.

References:

[1] Cheng, P. S., **Sun, J.**, Sun, S. N., Choi, A. Y., & Minnich, A. J. (2022). High-field transport and hot electron noise in GaAs from first principles: role of two-phonon scattering. _Physical Review B_, 106, 245201.

[2] **Sun, J.**, Minnich, A. J. (2023). Transport and noise of hot electrons in GaAs using a semi-analytical model of two-phonon polar optical phonon scattering.. _arXiv_ 2302.01480.

