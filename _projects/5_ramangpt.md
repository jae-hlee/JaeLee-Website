---
layout: page
title: RamanGPT
description: Bidirectional ML between crystal structures and Raman spectra
img: assets/img/projects/ramangpt.png
importance: 5
category: Research
related_publications: false
---

**RamanGPT** establishes a *bidirectional* mapping between crystal structures and Raman spectra. A *forward* model, a graph neural network (ALIGNN), predicts a Raman spectrum directly from a crystal structure. An *inverse* workflow recovers structure from a spectrum by matching it against a computational Raman database (cosine similarity) and generating candidate structures with a fine-tuned generative transformer (AtomGPT), which are then relaxed with an ML force field (ALIGNN-FF). Trained on a database of ~5,000 first-principles (DFPT) spectra, the goal is to make Raman a faster, more quantitative structural probe.

This work is described in *RamanGPT: Bidirectional Mapping Between Crystal Structures and Raman Spectra with Graph Neural Networks and Generative Transformers* ([arXiv:2606.03764](https://arxiv.org/abs/2606.03764)).
