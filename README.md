---
title: "Create R package with RStudio"
author: Jingyu Bao
date: 2017-03-03
---

# Framework

There are lots of sources about build R packages. Here is a simple intro for create one with RStudio and with Rcpp.

## Requirements

install [R](https://www.r-project.org/) and [RStudio](https://www.rstudio.com/) or [RStudio-server](https://www.rstudio.com/products/rstudio/download-server/)

In R, install _Rcpp_ package.
```
install.packages("Rcpp")
```

## Procedure

1. Click **File** -> **New Project**
2. **New Directory** -> **R Package**
3. Choose **type** to be _R package_ or _R package with Rcpp_.

## Modify your package

* add R script file into _./R_ folder
* add Rcpp script file into _./src_ folder

## Compile your package

You can find following info in the sample hello.R
>   Some useful keyboard shortcuts for package authoring:

>   Build and Reload Package:  'Ctrl + Shift + B'
>   Check Package:             'Ctrl + Shift + E'

Then click **Build** -> **Build Source Package**

## Install your package in other machine

in R, you can write
```
install.packages("packageName", repos = NULL, type = "source")
```
# References

[RStudio](https://support.rstudio.com/hc/en-us/articles/200486488-Developing-Packages-with-RStudio)
[Rcpp Package](https://support.rstudio.com/hc/en-us/articles/200486088-Using-Rcpp-with-RStudio)
[R package](http://r-pkgs.had.co.nz/)
