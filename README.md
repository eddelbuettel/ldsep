
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ldsep: Linkage Disequilibrium Shrinkage Estimation for Polyploids

<!-- badges: start -->

[![Lifecycle:
maturing](https://img.shields.io/badge/lifecycle-maturing-blue.svg)](https://www.tidyverse.org/lifecycle/#maturing)
[![R build
status](https://github.com/dcgerard/ldsep/workflows/R-CMD-check/badge.svg)](https://github.com/dcgerard/ldsep/actions)
[![Codecov test
coverage](https://codecov.io/gh/dcgerard/ldsep/branch/master/graph/badge.svg)](https://codecov.io/gh/dcgerard/ldsep?branch=master)
[![CRAN
status](https://www.r-pkg.org/badges/version/ldsep)](https://CRAN.R-project.org/package=ldsep)
[![](http://cranlogs.r-pkg.org/badges/grand-total/ldsep)](https://cran.r-project.org/package=ldsep)
[![License: GPL
v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
<!-- badges: end -->

Estimate haplotypic or component pairwise linkage disequilibrium (LD),
using either genotypes or genotype likelihoods. Support is provided to
estimate the popular measures of LD: the LD coefficient \(D\), the
standardized LD coefficient \(D'\), and the Pearson correlation
coefficient \(r\). All estimates are returned with corresponding
standard errors. These estimates and standard errors can be used for
shrinkage estimation. The methods are described in Gerard (2020).

The main functions are:

  - `ldest()`: Estimates pairwise LD.
  - `mldest()`: Iteratively apply `ldest()` across many pairs of SNPs.
  - `plot.lddf()`: Plot method for the output of `mldest()`.
  - `format_lddf()`: Format the output of `mldest()` into a matrix.
  - `ldshrink()`: Shrink correlation estimates using adaptive shrinkage
    (Stephens, 2017; Dey and Stephens, 2018).

## Installation

You can install the released version of ldsep from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("ldsep")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("dcgerard/ldsep")
```

## Code of Conduct

Please note that the ldsep project is released with a [Contributor Code
of
Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html).
By contributing to this project, you agree to abide by its terms.

## References

  - Dey, Kushal K., and Matthew Stephens. “CorShrink: Empirical Bayes
    shrinkage estimation of correlations, with applications.” *bioRxiv*
    (2018): 368316.
  - Gerard, David. “Pairwise Linkage Disequilibrium Estimation for
    Polyploids.” *Unpublished manuscript* (2020).
  - Stephens, Matthew. “False discovery rates: a new deal.”
    *Biostatistics* 18, no. 2 (2017): 275-294.
