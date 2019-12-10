# Drat Repository for github.com/schochastics

This contains the latest stable builds of my R packages that aren't available on CRAN (and probably never will be). So far, only the `networkdata` package is available, which has too much data and too few functions to be a CRAN candidate. The benefit of a drat archive like this is that you can install and upgrade non-CRAN packages directly from R using the standard install.packages() and update.packages() functions. E.g.,

```{r}
if (!require("drat")) {
    install.packages("drat")
}
drat::addRepo("schochastics")
install.packages("networkdata")
```
