
# WORCS <a href='https://osf.io/zcvbs/'><img src='paper/worcs_icon.png' align="right" height="139" /></a>

<!-- README.md is generated from README.Rmd. Please edit that file -->

<!--[![CRAN status](https://www.r-pkg.org/badges/version/worcs)](https://cran.r-project.org/package=worcs)
[![](https://cranlogs.r-pkg.org/badges/worcs)](https://cran.r-project.org/package=worcs)-->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Travis build
status](https://travis-ci.org/cjvanlissa/worcs.svg?branch=master)](https://travis-ci.org/cjvanlissa/worcs)
<!--[![Codecov test
coverage](https://codecov.io/gh/cjvanlissa/worcs/branch/master/graph/badge.svg)](https://codecov.io/gh/cjvanlissa/worcs?branch=master)-->
<!--[![DOI](http://joss.theoj.org/papers/10.21105/joss.00978/status.svg)](https://doi.org/10.21105/joss.00978)-->

The Workflow for Open Reproducible Code in Science (WORCS) is an easy to
adopt approach to ensuring a research project meets the requirements of
Open Science from the start. It is based on a “good enough” philosophy,
prioritizing user-friendliness over exhaustiveness. It can be used
either in absence of, or in parallel to, existing requirements for Open
workflows. It can also be enhanced with more elaborate solutions for
specific issues.

## Where do I start?

For most users, the recommended starting point is to read [the preprint
paper, available on the Open Science Framework](https://osf.io/zcvbs/).

The paper describes the WORCS workflow, and how the `worcs` package fits
into that workflow.

## About this repository

This repository contains the following:

1.  An R-package called `worcs`, with convenience functions to
    facilitate the WORCS workflow.
2.  In the subfolder `./paper`, the source files for the paper
    describing the WORCS workflow.

The repository serves two functions: To allow users to install the
`worcs` package, and to allow collaborators access to the source code
for the package and paper.

## Repository structure

| File          | Description                     | Usage           |
| :------------ | :------------------------------ | :-------------- |
| \_pkgdown.yml | YAML for package website        | do not edit     |
| DESCRIPTION   | R-package DESCRIPTION           | do not edit     |
| LICENSE.md    | Project license                 | do not edit     |
| NAMESPACE     | R-package namespace             | machine-written |
| README.md     | Read this file to get started\! | do not edit     |
| README.Rmd    | R-markdown source for readme.md | human editable  |
| worcs.Rproj   | Rstudio project file            | do not edit     |
| docs/         | Package website                 | machine-written |
| inst/         | Rstudio project template files  | human editable  |
| man/          | R-package documentation         | do not edit     |
| paper/        | WORCS paper source files        | human editable  |
| R/            | R-package source code           | human editable  |
| vignettes/    | R-package vignettes             | human editable  |

## Installing the package

Before installing the package, please read [this
vignette](https://cjvanlissa.github.io/worcs/articles/setup.html), which
explains how to set up your computer for `worcs`.

After reading [the
vignette](https://cjvanlissa.github.io/worcs/articles/setup.html), you
can install the development version of the `worcs` package from GitHub
with:

``` r
if(!requireNamespace("remotes"))install.packages("remotes")
remotes::install_github("cjvanlissa/worcs", dependencies = TRUE, update = "never")
remotes::install_github("crsh/papaja", dependencies = TRUE, update = "never")
tinytex::install_tinytex()
worcs::git_credentials("your_name", "your_email")
```

## Citing WORCS

You can cite WORCS using the following citation (please use the same
citation for either the package, or the paper):

> Van Lissa, C. J. (2020, February 11). WORCS: A Workflow for Open
> Reproducible Code in Science. <https://doi.org/10.17605/OSF.IO/ZCVBS>

## Contributing and Contact Information

WORCS is actively recruiting collaborators with valuable expertise, to
improve both the workflow and the package. Relevant contributions
warrant coauthorship to the paper. Please contact the lead author at
<c.j.vanlissa@uu.nl>, or:

  - File a GitHub issue [here](https://github.com/cjvanlissa/worcs)
  - Make a pull request
    [here](https://github.com/cjvanlissa/worcs/pulls)

By participating in this project, you agree to abide by the [Contributor
Code of Conduct v2.0](https://www.contributor-covenant.org/).

## Acknowledgements

The worcs logo is inspired by the Open Science Badges by the Center for
Open Science (CC-BY-4.0), and makes use of the gear, services, gears,
preferences, settings icon, made by MD Badsha Meah from www.freeicons.io
(CC-BY-3.0).
