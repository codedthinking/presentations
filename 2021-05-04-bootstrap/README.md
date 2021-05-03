---
title: "Bootstrapping Stata estimators with Make"
author: 
 - Miklós Koren
aspectratio: 54
---

# Problem
## Problem
* You have a complex estimator in a long Stata .do file.
* You cannot derive the standard errors analytically.

## The Stata solution
* `bs: regress outcome variables`
* But this only works for small estimation procedures, not if you have many data manipulation steps in between.
* Cannot be parallelized and may take a long time to run.

# The Make solution
## The Make solution

### Every estimator
data $\to$ estimator $\to$ statistic

### Every Make recipe
prerequisites $\to$ recipe $\to$ target

## The Make solution
* If `data`, `estimator` and `statistic` are in separate files, we can exploit the power of Make.
* `estimator` can be however complex, as long as it reads `data` and write `statistic`.
* The bootstrap repetitions can be run in parallel.

## Cookie cutter boostrap
[GitHub repo](https://github.com/codedthinking/cookiecutter-bootstrap-stata)