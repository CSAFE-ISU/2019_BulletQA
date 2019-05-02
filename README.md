
# 2019 REU: Bullet Scan QA

<!-- badges: start -->

<!-- badges: end -->

This project will involve the creation of a curated data set with
bullets that have been annotated, with the goal of ensuring that the
data used to fit a random forest for bullet matching is of the highest
possible quality.

You will annotate the scanned bullets, use `x3ptools` to view the
annotated bullets, and use `bulletxtrctr` to ensure that the features
derived from the bullet scan are optimal.

## Background Reading and Preparation Activities

### Github

This summer, you’ll be using GitHub to keep track of code and other work
you perform. Please create a github account if you haven’t already, and
send your username to Susan so you can be added to the CSAFE group.
[Happy Git and GitHub for the useR](https://happygitwithr.com/) is a
good online book that discusses how Git and R can be used together. The
`usethis` package in R makes using git and github in R projects
relatively stress-free.

### R setup

Please make sure you have R version 3.5.0 or above, and run
`update.packages(ask = FALSE, checkBuilt = TRUE)` to ensure your
packages are updated to the newest version.

You will need, at a minimum, the packages in the `tidyverse`,
`x3ptools`, and `bulletxtrctr`. To get these installed, run the
following commands:

``` r
install.packages("tidyverse", dependencies = c("suggests", "depends"))
install.packages("x3ptools", dependencies = c("suggests", "depends"))
install.packages("devtools")
devtools::install_github("heike/bulletxtrctr")
```

### Browser setup

CSAFE has developed a chrome extension for annotating x3p files, called
[fix3p](https://chrome.google.com/webstore/detail/fix3p/). Please
install the extension, and enable file support and debugging as
described in the installation instructions.

### Forensic Firearm and Toolmark Examination

  - Original bullet RF paper
  - case study validation paper
  - ??

## Getting Started

## Step 1: Annotations

We will use the following bullet scan data sets for fitting the random
forest:

  - Hamby 36
  - Hamby 44
  - Houston FSI
  - Phoenix PD
  - ??

In order to annotate the scans, you will load the x3p file into fix3p in
chrome, using the annotation tool to mark the following: - left groove -
right groove - breakoff - pitting - well-expressed striae

Examples of these issues are shown below:
