# sigident (!!! currently under development !!!)

<!-- badges: start -->
[![pipeline status](https://gitlab.miracum.org/clearly/sigident/badges/master/pipeline.svg)](https://gitlab.miracum.org/clearly/sigident/commits/master)
[![coverage report](https://gitlab.miracum.org/clearly/sigident/badges/master/coverage.svg)](https://gitlab.miracum.org/clearly/sigident/commits/master)
<!-- badges: end -->

This is the repository of the R package 'sigident'. It provides core functionalities to identify diagnostic and prognostic signatures from gene expression datasets.

Currently implemented features are:

- merging of microarray datasets
- DEG analysis
- functional analysis (gene enrichment)
- Identification of diagnostic signatures, using
  + Lasso regression
  + Elastic net regression
  + glmnet (grid search for best alpha and lambda)
- Identification of prognostic signatures

## Installation

You can install the development version of *sigident* with:

``` r
options('repos' = 'https://ftp.fau.de/cran/')
install.packages("devtools")
devtools::install_git("https://gitlab.miracum.org/clearly/sigident.git")
```

## Example

Please view the package's vignette to see a detailled description how to perform merging, signature and functional analyses of microarray data.

## Citation  

To cite the 'sigident' package in publications, please use: 

```
@Article{,
    title = {A Toolbox for Functional Analysis and the Systematic Identification of Diagnostic and Prognostic Gene Expression Signatures Combining Meta-Analysis and Machine Learning},
    volume = {11},
    doi = {10.3390/cancers11101606},
    pages = {14},
    number = {1606},
    journal = {Cancers},
    author = {Johannes Vey and Lorenz A. Kapsner and Maximilian Fuchs and Philipp Unberath and Giulia Veronesi and Meik Kunz},
    year = {2019},
}
```
and

```
@Manual{,
    title = {sigident: Signature Analyses in Genomic Expression Sets},
    author = {Lorenz A. Kapsner and Johannes Vey and Meik Kunz and Andreas Pittroff},
    year = {2019},
    note = {R package version 0.0.1.9000},
    url = {https://gitlab.miracum.org/clearly/sigident},
}
```
