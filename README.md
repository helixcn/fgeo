
<!-- README.md is generated from README.Rmd. Please edit that file -->

# <img src="https://i.imgur.com/m8FNhQR.png" align="right" height=88 /> fgeo: Analyze forest diversity and dynamics

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Travis build
status](https://travis-ci.org/forestgeo/fgeo.svg?branch=master)](https://travis-ci.org/forestgeo/fgeo)
[![Coverage
status](https://coveralls.io/repos/github/forestgeo/fgeo/badge.svg)](https://coveralls.io/r/forestgeo/fgeo?branch=master)
[![CRAN
status](https://www.r-pkg.org/badges/version/fgeo)](https://cran.r-project.org/package=fgeo)

**fgeo** installs and loads multiple packages, functions and datasets in
a single
step.

## Packages

| package                                                                 | title                                           |
| :---------------------------------------------------------------------- | :---------------------------------------------- |
| <a href=https://forestgeo.github.io/bciex>bciex</a>                     | Forest Dynamics Data from Barro Colorado Island |
| <a href=https://forestgeo.github.io/fgeo>fgeo</a>                       | Easily Install and Load Multiple Packages       |
| <a href=https://forestgeo.github.io/fgeo.abundance>fgeo.abundance</a>   | Calculate Abundance and Basal Area              |
| <a href=https://forestgeo.github.io/fgeo.demography>fgeo.demography</a> | Calculate Mortality, Recruitment and Growth     |
| <a href=https://forestgeo.github.io/fgeo.habitat>fgeo.habitat</a>       | Analize Soil Data                               |
| <a href=https://forestgeo.github.io/fgeo.map>fgeo.map</a>               | Map Species, Trees and Topography               |
| <a href=https://forestgeo.github.io/fgeo.tool>fgeo.tool</a>             | Functions for General Purposes                  |

## Search [functions and datasets](https://forestgeo.github.io/fgeo/articles/fgeo.html)

## Installation

    # install.packages("remotes")
    remotes::install_github("forestgeo/fgeo")

To learn the details about how to install packages from GitHub, read
[this blog post](https://goo.gl/dQKEeg).

## Example

Load all **fgeo** packages in one step.

``` r
library(fgeo)
```

Update packages that changed since last installation.

    fgeo_update()

Table packages.

``` r
fgeo_index_packages()
#>           package                                           Title
#> 1           bciex Forest Dynamics Data from Barro Colorado Island
#> 2            fgeo       Easily Install and Load Multiple Packages
#> 3  fgeo.abundance              Calculate Abundance and Basal Area
#> 4 fgeo.demography     Calculate Mortality, Recruitment and Growth
#> 5    fgeo.habitat                               Analize Soil Data
#> 6        fgeo.map               Map Species, Trees and Topography
#> 7       fgeo.tool                  Functions for General Purposes
```

Table and explore functions.

``` r
library(dplyr)
funs <- fgeo_index_functions()
sample_n(funs, 10)
#>            package                   fun
#> 74       fgeo.tool     fieldforms_output
#> 9             fgeo             fgeo_link
#> 94       fgeo.tool row_collapse_censusid
#> 103      fgeo.tool           type_ensure
#> 89       fgeo.tool    nms_restore_newvar
#> 93       fgeo.tool      restructure_elev
#> 76       fgeo.tool               fill_na
#> 91       fgeo.tool        recode_subquad
#> 8             fgeo   fgeo_index_packages
#> 14  fgeo.abundance       abundance_tally
```

## Related projects

Maintained by ForestGEO

  - [**fgeo.template**](https://forestgeo.github.io/fgeo.template/): An
    R package containing templates used to develop **fgeo** packages.

Not maintained by ForestGEO

  - [CTFS-R Package](http://ctfs.si.edu/Public/CTFSRPackage/): The
    original package of CTFS functions. No longer supported by
    ForestGEO.

  - [**BIOMASS**](https://CRAN.R-project.org/package=BIOMASS): An R
    package to estimate above-ground biomass in tropical
        forests.
    
      - [Description](https://CRAN.R-project.org/package=BIOMASS)
      - [Manual](https://cran.r-project.org/web/packages/BIOMASS/BIOMASS.pdf)
      - [Vignette](https://cran.r-project.org/web/packages/BIOMASS/vignettes/VignetteBiomass.html)

## Information

  - [Getting help](SUPPORT.md).
  - [Contributing](CONTRIBUTING.md).
  - [Contributor Code of Conduct](CODE_OF_CONDUCT.md).

## Acknowledgements

Thanks to all partners of ForestGEO, for sharing their ideas and code.
