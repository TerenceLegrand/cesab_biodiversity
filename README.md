<!-- README.md is generated from README.Rmd. Please edit that file -->

# cesab\_biodiversity <img src="man/figures/compendium-sticker.png" align="right" style="float:right; height:120px;"/>

<!-- badges: start -->

[![License: GPL (&gt;=
2)](https://img.shields.io/badge/License-GPL%20%28%3E%3D%202%29-blue.svg)](https://choosealicense.com/licenses/gpl-2.0/)
<!-- badges: end -->

<p align="left">
• <a href="#overview">Overview</a><br> •
<a href="#features">Features</a><br> •
<a href="#content">Content</a><br> •
<a href="#installation">Installation</a><br> •
<a href="#usage">Usage</a><br> • <a href="#citation">Citation</a><br> •
<a href="#contributing">Contributing</a><br> •
<a href="#acknowledgments">Acknowledgments</a><br> •
<a href="#references">References</a>
</p>

## Overview

This research compendium was created in order to map biodiversity facets (taxonomic, functional and phylogenetic) for both breeding birds and trees across the Euro-Mediterranean Basin. A sub-goal is to make the workflow as reproducible as possible.

## Features

The main purpose of this compendium was to make an already written workflow into a more comprehensive, coherent and reproducible project. 

## Content

This repository is structured as follow:

-   [`DESCRIPTION`](https://github.com/MCartereau/cesab_biodiversity/tree/main/DESCRIPTION):
    contains project metadata (authors, date, dependencies, etc.)

-   [`make.R`](https://github.com/MCartereau/cesab_biodiversity/tree/main/make.R):
    main R script to run the entire project

-   [`R/`](https://github.com/MCartereau/cesab_biodiversity/tree/main/R):
    contains R functions developed especially for this project

- [`data/`](https://github.com/MCartereau/cesab_biodiversity/tree/main/data):
contains raw- and derived-data.

Here you can view the functions and data as an inter-connected network using the **targets** R package : 

```{r, results = "asis", echo = FALSE}
cat(c("```{mermaid}", targets::tar_mermaid(), "```"), sep = "\n")
```



## Installation

To install this compendium:

-   [Fork](https://docs.github.com/en/get-started/quickstart/contributing-to-projects)
    this repository using the GitHub interface.
-   [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
    your fork using `git clone fork-url` (replace `fork-url` by the URL
    of your fork). Alternatively, open [RStudio
    IDE](https://posit.co/products/open-source/rstudio/) and create a
    New Project from Version Control.

## Usage

Launch the
[`make.R`](https://github.com/MCartereau/cesab_biodiversity/tree/main/make.R)
file with:

    source("make.R")

**Notes**

-   All required packages listed in the `DESCRIPTION` file will be
    installed (if necessary)
-   All required packages and R functions will be loaded
-   Some analyses listed in the `make.R` might take time

## Citation

Nothing yet...


## Contributing

All types of contributions are encouraged and valued. For more
information, check out our [Contributor
Guidelines](https://github.com/MCartereau/cesab_biodiversity/blob/main/CONTRIBUTING.md).

Please note that this project is released with a [Contributor Code of
Conduct](https://contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html).
By contributing to this project, you agree to abide by its terms.

## Acknowledgments

Thanks to Cesab !!

## References


> Marwick B, Boettiger C, Mullen L. 2018. Packaging data analytical work reproducibly using R (and friends) PeerJ Preprints 6:e3192v2 https://doi.org/10.7287/peerj.preprints.3192v2

> Casajus N, Bonnici I, Dray S, Gimenez O, Guéry L, Guilhaumon F, Schiettekatte NMD & Siberchicot A (2023) Workshop FRB-CESAB & RT EcoStat: Reproducible Research in Computational Ecology. Zenodo. http://doi.org/10.5281/zenodo.4262978.