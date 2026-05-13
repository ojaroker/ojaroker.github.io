---
layout: page
title: Count Regression Package
description: R Package for Count and Zero-Inflated Regression Modeling
img: assets/img/projects/glmOJ/illus.png
importance: 1
category: "2026"
related_publications: false
---

`glmOJ` is an R package providing a unified workflow for fitting, diagnosing, and interpreting count and semi-continuous regression models. It supports Poisson, quasi-Poisson, negative binomial, Tweedie, and their zero-inflated counterparts (ZIP, ZINB, ZI-Tweedie).

The package's main contribution is a general-purpose wrapper that automatically fits a family of base models, runs zero-inflation tests on each, conditionally fits the corresponding zero-inflated model, and selects the best fit by AIC, BIC, log-likelihood, or McFadden pseudo-R². It also includes data summarization tools and randomized quantile residual diagnostics via DHARMa. The package was developed as a final project for MATH 454 Statistical Learning. Full documentation and vignettes are available at the [package site](https://oscar.jaroker.com/glmOJ), and the source is on [GitHub](https://github.com/ojaroker/glmOJ).
