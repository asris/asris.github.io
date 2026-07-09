---
layout: page
title: Software & Tools
permalink: /software/
nav: false
nav_order: 9
description: Internal analysis pipelines and computational tooling built to support the research program. Most tools are currently unreleased; public repositories will be linked here as they mature.
---

## Overview

I develop and maintain a small set of internal, research-purpose analysis tools that support the quantitative arm of my program. None of these tools have been publicly released yet; this page will be updated as individual components mature and are cleared for public sharing.

If any of the workflows below would be useful in a specific project, please reach out — collaborative access is straightforward.

---

## Custom Python pipeline for HD-MEA and organoid electrophysiology

Analysis and visualization layer built on top of MaxWell Biosystems' MaxLab Live / MaxLive export format. Handles day-of-recording QC and post-hoc summarization for MaxOne PLM and PSM MEA chips.

**Capabilities.**

- Spatial firing-rate mapping across the electrode grid, with per-channel classification (silent < 5 Hz, slow 5–50 Hz, fast > 50 Hz).
- Spike-amplitude and inter-spike-interval (ISI) distribution modelling, including bi-/uni-modal fits.
- Kernel-density estimation of population firing structure.
- Pharmacology-aware comparison (e.g., pre- and post-bicuculline).

*Status: internal, in active development. No public release yet.*

---

## MATLAB biomarker-trajectory workflows

MATLAB scripts for modelling longitudinal biomarker response to therapeutic exposure — used across the α-synuclein / Aβ / mitochondrial-injury panels. The workflow ingests plate-reader and JESS output, fits fold-change and dose–response models with appropriate multiple-comparison structure (ANOVA with Bonferroni or Tukey post-hoc), and produces figure-ready summary plots aligned to PK/PD sampling schedules.

*Status: internal, in active development. No public release yet.*

---

## Statistical stack in daily use

- **GraphPad Prism**, **OriginLab Pro**, **ImageJ / Fiji** (with the CellProfiler pipeline for high-content imaging quantification).
- **Python** (NumPy, pandas, SciPy, matplotlib, seaborn) and **MATLAB** for custom analysis and modelling.

---

*Public code releases will be published via my [GitHub profile](https://github.com/asris) as they become available.*
