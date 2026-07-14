---
layout: page
title: DiffractGPT-Rietveld
description: Automated crystal structure determination from powder XRD
img: assets/img/projects/diffractgpt.png
importance: 7
category: Research
related_publications: false
---

**DiffractGPT-Rietveld** is an automated pipeline for determining crystal structures from powder X-ray diffraction (XRD) data. It pairs generative machine-learning structure prediction (DiffractGPT) with database pattern matching and computational Rietveld refinement. For a known material it matches the measured pattern against reference structures, and for a novel compound it generates candidate structures directly from the diffraction pattern and then refines the lattice parameters. Benchmarked on mineral samples and crystal-structure datasets, it recovers lattice parameters with success rates of roughly 80 to 98 percent, and it runs as an open, web-accessible tool on [AtomGPT.org](https://atomgpt.org).

This work is described in *Hybrid DiffractGPT-Rietveld Refinement Framework for Automated X-ray Diffraction Analysis* ([arXiv:2607.08890](https://arxiv.org/abs/2607.08890)).
