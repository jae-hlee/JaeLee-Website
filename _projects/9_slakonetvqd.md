---
layout: page
title: SlaKoNet-VQD
description: Variational quantum band structures from neural tight-binding Hamiltonians
img: assets/img/projects/slakonetvqd.png
importance: 9
category: Research
related_publications: false
---

**SlaKoNet-VQD** couples the SlakoNet neural tight-binding model with variational quantum algorithms to compute electronic band structures on near-term quantum hardware. Variational methods such as VQE and VQD are promising for periodic solids, but their reach is limited by the cost of building a faithful second-quantized Hamiltonian, which typically requires DFT plus Wannierization or hand-fit tight-binding parameters. SlaKoNet-VQD replaces that step with a universal neural Hamiltonian generator spanning 65 elements, giving a workflow that is structure-agnostic, differentiable, and suited to high-throughput band-structure screening. Benchmarks recover the full eight-band structure of silicon to within about 2 meV of exact diagonalization on a 3-qubit simulator, extend to five conventional superconductors (Al, Ta, Nb, V, ZrN), and include a ground-state calculation on aluminum executed on real IBM Quantum hardware. The Hamiltonian can further be promoted to a correlated Hubbard model solved with dynamical mean-field theory, pointing to the impurity problem as a natural target for quantum solvers.

This work is described in *SlaKoNet-VQD: A Universal Slater-Koster Tight-Binding Hamiltonian for Variational Quantum Band-Structure Calculations on Near-Term Hardware* ([arXiv:2607.09761](https://arxiv.org/abs/2607.09761)).
