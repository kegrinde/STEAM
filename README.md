---
title: STEAM
author: Kelsey Grinde
output:
  md_document:
    variant: markdown_github
---

<!-- README.md is generated from README.Rmd. Please edit that file -->



# Introduction

STEAM (Significance Threshold Estimation for Admixture Mapping) is an R package which contains various functions relevant to estimating genome-wide significance thresholds for admixture mapping studies. 

This package is under active development and we are in the process of submitting a manuscript which contains details regarding the methods implemented here. Please stay tuned for future updates!

# Examples

## Analytic Approximation

For an admixture mapping study in an admixed population with two ancestral populations (e.g., African Americans), we can use an analytic approximation to the family-wise error rate to quickly compute a genome-wide significance threshold for our study. 

Suppose you are conducting an admixture mapping study in an admixed population with 2 ancestral populations, 6 generations since admixture, and markers spaced every 0.2 cM (on average) across 22 chromosomes of total length 3500 cM. To estimate the *p*-value threshold which will control the family-wise error rate for this study at the 0.05 level, use the following command:


```r
get_thresh_analytic(g = 6, delt = 0.2, L = 3500, type = "pval")
#> [1] 1.887352e-05
```

## Test Statistic Simualtion

Coming soon!

## Estimating the Number of Generations since Admixture

Coming soon!