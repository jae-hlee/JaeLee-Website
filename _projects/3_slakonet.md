---
layout: page
title: SlaKoNet DB
description: ML electronic-property prediction at scale
img: assets/img/projects/slakonet.png
importance: 3
category: Research
related_publications: false
---

This project benchmarks machine-learning models for predicting electronic properties — primarily band gaps — across **millions of crystal structures** drawn from the Alexandria (3D, 2D, 1D) and JARVIS databases plus molecular sets. Two complementary approaches are compared:

- **SlakoNet** — a Slater–Koster tight-binding neural network that is interpretable and yields a density of states, and
- **ALIGNN** — an atomistic line-graph neural network that achieves higher accuracy as a black-box predictor.

The study quantifies where each model excels and fails (e.g., transition-metal and fluoride chemistries), and shows that structural geometry — bulk crystals versus slabs — can matter more than the model architecture itself. The result is a practical map of when interpretable physics-based models are "good enough" versus when accuracy demands a graph neural network.
