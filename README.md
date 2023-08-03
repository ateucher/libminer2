
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer2

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer2 is to provide a summary of a user’s R libraries.
It’s a toy package developed in a workshop and not meant for serious
use.

## Installation

You can install the development version of libminer2 from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("ateucher/libminer2")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer2)

lib_summary()
#>                                                                                       library
#> 1                        /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
#> 2 /private/var/folders/_f/n9fw7ctx3fqf2ty9ylw502g80000gn/T/RtmpwFb5IO/temp_libpath412b23e2494
#> 3                                                     /Users/andy/Library/R/arm64/4.3/library
#>   n_packages
#> 1         29
#> 2          1
#> 3        200

# You can also ask it to calculate sizes:
lib_summary(sizes = TRUE)
#>                                                                                       library
#> 1                        /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
#> 2 /private/var/folders/_f/n9fw7ctx3fqf2ty9ylw502g80000gn/T/RtmpwFb5IO/temp_libpath412b23e2494
#> 3                                                     /Users/andy/Library/R/arm64/4.3/library
#>   n_packages   lib_size
#> 1         29   71351828
#> 2          1      14424
#> 3        200 1174761571
```
