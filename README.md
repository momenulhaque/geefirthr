# geefirth

<!-- badges: start -->
<!-- badges: end -->

The goal of geefirth is to fit Generalized Estimating Equation (GEE) for  correlated binary data with separation or near-to-separation

## Installation

You can install the development version of geefirth like so:

``` r
devtools::install_github("momenulhaque/geefirth") # it will install the package

```

## Example

This is a basic example which shows you how to fit a GEE on a data set

```{r example}
library(geefirth)
## basic example code

data(geefirth)

# Fitting GEE for quasi-separated data

geefirth(y ~ x + obstime, id=id, data=quasiDat, corstr = "exchangeable")

# Fitting GEE for near to quasi-separated data

geefirth(y ~ x + obstime, id=id, data=nearDat, corstr = "exchangeable")


```


