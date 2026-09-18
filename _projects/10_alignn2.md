---
layout: page
title: ALIGNN 2.0
description: One graph network for properties, force fields, inverse design, spectra, and microscopy
img: assets/img/projects/alignn2.png
importance: 1
category: Research
related_publications: false
---

**ALIGNN 2.0** is a dependency-free, pure-PyTorch reimplementation of the Atomistic Line Graph Neural Network, with the line graph and its batching built from scratch so that it runs on current-generation accelerators without a specialized graph library. A crystal structure becomes an atom graph and a line graph whose nodes are bonds and whose edges carry bond angles. Edge-gated message passing alternates between the two graphs, and one shared per-atom representation feeds every output head: scalar properties, spectra and tensors, per-atom charges and magnetic moments, and energies whose gradients give forces and stress for molecular dynamics. Comparing graph constructions, the wider k-nearest-neighbor graph is more accurate for properties while the smoothly varying radius graph is required for energy-conserving dynamics.

On the JARVIS-Leaderboard, ALIGNN 2.0 leads on 26 of 30 single-property benchmarks against the original ALIGNN, with the largest gains for piezoelectric and dielectric maxima, exfoliation energy, elastic moduli, and superconducting transition temperature. The LAMMPS- and OpenMM-compatible ALIGNN-FF force field matches leading universal potentials on the Matbench-Discovery and CHIPS-FF benchmarks with a small fraction of their parameters and scales to hundred-thousand-atom cells. The same network serves as the denoiser in a conditional crystal-diffusion model for inverse design, and from a single relaxed structure it reconstructs infrared, Raman, optical-dielectric, and neutron spectra and drives frozen-phonon electron-microscopy image simulation.

This work is described in *ALIGNN 2.0: A Unified Line-Graph Neural Network Framework for Materials Screening, Force Fields, Inverse Design, Spectroscopy, and Microscopy* ([arXiv:2609.19487](https://arxiv.org/abs/2609.19487)).

**Demo:** [atomgpt.org/alignn](https://atomgpt.org/alignn)

**Code:** [github.com/atomgptlab/alignn](https://github.com/atomgptlab/alignn)
