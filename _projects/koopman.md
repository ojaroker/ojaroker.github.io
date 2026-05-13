---
layout: page
title: Koopman Analysis of Chua's Circuit
description: EDMD Applied to a Physical Chaotic System
img: assets/img/projects/koopman/illus.png
importance: 1
category: "2026"
related_publications: false
pdf: KoopmanChua.pdf
---

Chua's Circuit is one of the simplest electronic circuits known to exhibit chaos. This project applies the Extended Dynamic Mode Decomposition (EDMD) algorithm to experimentally collected time-series data from a physical Chua's Circuit to approximate the Koopman operator — an infinite-dimensional linear operator that governs the evolution of observable functions along nonlinear trajectories.

The circuit was built in lab and data was collected using an Arduino microcontroller across four dynamical regimes: fixed point, limit cycle, period-doubled, and double scroll (chaotic). EDMD was used to construct a finite-dimensional approximation of the Koopman operator using polynomial and radial basis function dictionaries. The resulting eigenvalues and eigenfunctions reveal the dominant frequencies and geometric structure of each regime. The double scroll attractor was analyzed further using Lyapunov exponent estimation, correlation dimension, and box-counting dimension. The MATLAB code is on [GitHub](https://github.com/ojaroker/Koopman-DMD).
