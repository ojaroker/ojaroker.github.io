---
layout: page
title: Optimal Harvesting
description: Stochastic Predator-Prey Environment
img: assets/img/projects/predator_prey/illus.jpg
importance: 1
category: Personal
related_publications: false
pdf: MCMReport.pdf
---

Abstract: We study the problem of optimally harvesting two interacting species—one a predator of the other—modeled using a stochastic Lotka–Volterra system with harvesting. The objective is to maximize total expected revenue from fishing both species over a finite time horizon, accounting for nonlinear extraction costs and environmental stochasticity. We derive the necessary conditions for optimality using the stochastic maximum principle in cases where the diffusion is and is not dependent on the control. Where analytical solutions are intractable, we employ a forward-backward sweep method to compute the optimal harvesting strategy numerically. The paper concludes with simulations and comparisons with linearized and deterministic approximations.

This project is currently in progress. Most of the theoretical work has been done; the current challenge is figuring out an appropriate method to solve the backward SDEs. The in-development code is [here](https://github.com/ojaroker/OptimalHarvesting).
