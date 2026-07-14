---
layout: page
title: Hallucination Detector
description: LLM and Semantic Scholar citation verification for scientific literature
img: assets/img/projects/hallucination.png
img_class: tile-img-pad
importance: 8
category: Research
related_publications: false
---

**Hallucination Detector** is an open, web-accessible tool that checks whether the citations in scientific writing are real. As large language models are increasingly used to draft manuscripts, fabricated references (invented authors, bogus DOIs, and citations stitched together from several genuine papers) have begun slipping into the published literature. The tool combines LLM-based extraction of each reference's bibliographic fields with structured retrieval from Semantic Scholar. It pulls the closest matching real papers and scores the agreement across title, authorship, and venue to grade each citation as trustworthy, partially supported, or likely fabricated. Benchmarked against a curated set of confirmed hallucinated citations from accepted NeurIPS 2025 papers, it flags the large majority of them, and it runs on [AtomGPT.org](https://atomgpt.org).

This work is described in *Hallucination Detector: A Hybrid LLM and Semantic Scholar Tool-Calling System for Detecting Hallucination in Scientific Literature on AtomGPT.org* ([arXiv:2607.09774](https://arxiv.org/abs/2607.09774)).
