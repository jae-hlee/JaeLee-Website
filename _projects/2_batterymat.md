---
layout: page
title: BatteryMat
description: ML-accelerated DFT screening of battery cathodes
img:
importance: 2
category: Research
related_publications: false
---

**BatteryMat** is a computational pipeline for designing lithium-ion (and beyond-lithium) battery electrodes. It moves candidates through a funnel: high-throughput screening of tens of thousands of structures across multiple working ions (Li, Na, K, Ca, Mg, Al, Zn), voltage and thermodynamic-stability filtering, composite-score ranking of cathode candidates, and then sequential DFT supercell delithiation to compute voltage curves and convex-hull stability. It also estimates ion-migration kinetics via nudged elastic band (NEB) barriers and benchmarks against known materials such as LFP, LMO, LCO, and NMC.

A parallel effort scales the ML screening stage to millions of structures (Alexandria database, 14 working ions). The methods combine VASP DFT, ML interatomic potentials (ALIGNN-FF), and automated thermodynamic analysis.

Presented as a poster at the **NIST Quantum Matters in Materials Science (QMMS) Workshop** (Gaithersburg, MD).
