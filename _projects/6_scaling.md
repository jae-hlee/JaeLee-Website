---
layout: page
title: GPU Scaling for Materials
description: Benchmarking DFT &amp; ML force fields on Blackwell GPUs
img: assets/img/projects/scaling.png
importance: 6
category: Research
github: https://github.com/jae-hlee/scaling_jae
related_publications: false
---

Large-scale materials simulation is only useful if it runs fast and stays numerically trustworthy. This project benchmarks two workloads on NVIDIA Blackwell **B200** GPUs: ML-force-field (ALIGNN-FF) inference on copper supercells from a few atoms up to ~780k atoms, and VASP DFT self-consistent-field scaling on silicon supercells. Along the way it characterizes a float32 energy-drift "cliff" near ~470k atoms that bounds the safe single-precision operating window, and measures strong- and size-scaling behavior to inform how big a simulation can responsibly go.
