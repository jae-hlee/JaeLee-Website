---
layout: page
title: BatteryMat
description: ML-accelerated DFT screening of battery cathodes
img: assets/img/projects/batterymat.png
importance: 2
category: Research
related_publications: true
---

**BatteryMat** is a computational pipeline for designing lithium-ion (and beyond-lithium) battery electrodes. It moves candidates through a funnel: high-throughput screening of tens of thousands of structures across multiple working ions (Li, Na, K, Ca, Mg, Al, Zn), voltage and thermodynamic-stability filtering, composite-score ranking of cathode candidates, and then sequential DFT supercell delithiation to compute voltage curves and convex-hull stability. It also estimates ion-migration kinetics via nudged elastic band (NEB) barriers and benchmarks against known materials such as LFP, LMO, LCO, and NMC {% cite lee2026batterymat %}.

A parallel effort scales the ML screening stage to millions of structures (Alexandria database, 14 working ions). The methods combine VASP DFT, ML interatomic potentials (ALIGNN-FF), and automated thermodynamic analysis.

This work is described in *BatteryMat: A Hierarchical Machine-Learning and DFT Framework for Average-Voltage Screening of Lithium-Ion Cathode Materials* ([arXiv:2607.06645](https://arxiv.org/abs/2607.06645)). The three-tier pipeline screens with ALIGNN, validates with a machine-learning force field, and finishes with DFT using automatically selected exchange-correlation functionals. It reproduces commercial lithium-ion voltages within 0.3 V and volumetric capacity within 5 percent, and it flags 71 JARVIS-DFT and 213 Alexandria structures as new cathode candidates.

Presented as a poster at the **NIST Quantum Matters in Materials Science (QMMS) Workshop** (Gaithersburg, MD).

**Code:** [github.com/jae-hlee/batterymat_jae](https://github.com/jae-hlee/batterymat_jae)
