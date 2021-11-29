boundsheff
================

# Overview

boundsheff is an R package containing area boundaries for Sheffield as
[simple features](https://r-spatial.github.io/sf/articles/sf1.html).

# Installation

You can install the development version from GitHub with:

``` r
# install.packages("devtools")
devtools::install_github("scc-pi/boundsheff")
```

If you work for Sheffield City Council you can install the binary
package for Windows from:

> S:\\BI Team\\ShareToAll\\RPackages

Using RStudio you can does this via the *Tools \> Install packages…*
menu.

# Sources

The data is from the [ONS Open Geography
Portal](https://scc-pi.github.io/notes/spatial-data-sources.html#open-geography),
the [SCC AGOL](https://sheffieldcc.maps.arcgis.com/) (ArcGIS Online), or
the [SCC
Portal](https://sheffieldcitycouncil.cloud.esriuk.com/portal/home/)
(ArcGIS Enterprise). The latter is behind the Council’s firewall.

# Sheffield boundaries

``` r
library(boundsheff)
library(sf)
```

    ## Linking to GEOS 3.9.1, GDAL 3.2.1, PROJ 7.2.1

## sf_sheff

LA (Local Authority) boundary.

## sf_asc_localities

``` r
plot(st_geometry(sf_asc_localities))
```

![](README_files/figure-gfm/sf_asc_localities-1.png)<!-- -->
