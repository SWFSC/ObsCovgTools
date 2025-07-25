<!-- README.md is generated from README.Rmd. Please edit that file -->

# ObsCovgTools <img src="logo.png" width="200" height="231" align="right" style="padding: 10px"/>

<!-- badges: start -->

[![GitHub release (latest by
date)](https://img.shields.io/github/v/release/kacurtis/ObsCovgTools)](https://github.com/kacurtis/ObsCovgTools/releases)
[![DOI](https://zenodo.org/badge/131074481.svg)](https://zenodo.org/doi/10.5281/zenodo.3603463)
<!-- badges: end -->

### Description

ObsCovgTools provides tools for evaluating fishery observer coverage,
particularly with respect to documenting and estimating rare bycatch.
Current functionality includes evaluating observer coverage in terms of

1)  probabilities of observing a bycatch event and of any bycatch
    occurring in total effort, given mean bycatch rate, dispersion index
    (variance to mean ratio in the bycatch rate), and total fishery
    effort;
2)  upper confidence limit of bycatch when none was observed, given
    total fishery effort and dispersion index; and
3)  bycatch estimation CV (coefficient of variation), given bycatch
    rate, dispersion index, and total fishery effort.

Estimates in all cases are based directly on the corresponding Poisson
or negative binomial probability distribution.

### Caveat

The ObsCovgTools package assumes that

- observer coverage is representative,
- bycatch is in terms of individuals (not weight) per unit effort, and
- the specified dispersion index reflects the highest level of any
  hierarchical variance (e.g., using dispersion index at trip level if
  greater than that at set level).

Violating these assumptions may result in negatively biased projections
of observer coverage required to meet specific objectives. Users may
want to explore uncertainty in dispersion index and in bycatch per unit
effort by varying those inputs.

### Shiny app

This package has been implemented as a Shiny web application, coauthored
by Howard Coleman, which can be accessed at
<https://connect.fisheries.noaa.gov/ObsCovg/>

(If you encounter an error at that link, you can also try
<https://kacurtis.shinyapps.io/obscov/>)

### Installation

You can install or update {ObsCovgTools} from
[GitHub](https://github.com/kacurtis/ObsCovgTools) with:

``` r
# install.packages("devtools")
remotes::install_github("kacurtis/ObsCovgTools")
```

### Citation

If you use ObsCovgTools results in publications or talks, please cite
the primary citation:

Curtis K. A., Carretta J. V. 2020. ObsCovgTools: Assessing observer
coverage needed to document and estimate rare event bycatch. Fisheries
Research, 225: 105493. <https://doi.org/10.1016/j.fishres.2020.105493>

You can also cite the package, updating the version number and year if
you use a more recent version:

Curtis K. A. 2020. ObsCovgTools: Evaluate Fishery Observer Coverage for
Bycatch Estimation. R package version 3.1.1.
<https://kacurtis.github.io/ObsCovgTools>

### Funding

Development of the ObsCovgTools package and the Shiny application was
supported by a grant from the National Marine Fisheries Service (NMFS)
Office of Science and Technology, through a contract to Ocean
Associates, Inc. 

<!-- Do not edit below. This adds the Disclaimer and NMFS footer. -->

------------------------------------------------------------------------

**Disclaimer** This repository is a scientific product and is not
official communication of the National Oceanic and Atmospheric
Administration, or the United States Department of Commerce. All NOAA
GitHub project code is provided on an ‘as is’ basis and the user assumes
responsibility for its use. Any claims against the Department of
Commerce or Department of Commerce bureaus stemming from the use of this
GitHub project will be governed by all applicable Federal law. Any
reference to specific commercial products, processes, or services by
service mark, trademark, manufacturer, or otherwise, does not constitute
or imply their endorsement, recommendation or favoring by the Department
of Commerce. The Department of Commerce seal and logo, or the seal and
logo of a DOC bureau, shall not be used in any manner to imply
endorsement of any commercial product or activity by DOC or the United
States Government.

------------------------------------------------------------------------

<img src="https://raw.githubusercontent.com/nmfs-general-modeling-tools/nmfspalette/main/man/figures/noaa-fisheries-rgb-2line-horizontal-small.png" width="200" style="height: 75px !important;"  alt="NOAA Fisheries">

[U.S. Department of Commerce](https://www.commerce.gov/) \| [National
Oceanographic and Atmospheric Administration](https://www.noaa.gov) \|
[NOAA Fisheries](https://www.fisheries.noaa.gov/)
