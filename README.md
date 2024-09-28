
<!-- README.md is generated from README.Rmd. Please edit that file -->

# my-GEO712-repository

<!-- badges: start -->
<!-- badges: end -->

The goal of my-GEO712-repository is to learn how to work with GitHub

## Last week’s project

Here is my previous activity:

``` r
#install.packages(c("here","usethis","annotater"))
library(here)
#> here() starts at /Users/esingurcan/Desktop/GEO 712/my-GEO712-repository/my-GEO712-repository
library(usethis)
library(annotater)
```

## Review the status

``` r
renv::status()
#> The following package(s) are in an inconsistent state:
#> 
#>  package     installed recorded used
#>  annotater   y         n        y   
#>  askpass     y         n        y   
#>  base64enc   y         n        y   
#>  bit         y         n        y   
#>  bit64       y         n        y   
#>  bslib       y         n        y   
#>  cachem      y         n        y   
#>  cli         y         n        y   
#>  clipr       y         n        y   
#>  cpp11       y         n        y   
#>  crayon      y         n        y   
#>  credentials y         n        y   
#>  curl        y         n        y   
#>  desc        y         n        y   
#>  digest      y         n        y   
#>  dplyr       y         n        y   
#>  evaluate    y         n        y   
#>  fansi       y         n        y   
#>  fastmap     y         n        y   
#>  fontawesome y         n        y   
#>  fs          y         n        y   
#>  generics    y         n        y   
#>  gert        y         n        y   
#>  gh          y         n        y   
#>  gitcreds    y         n        y   
#>  glue        y         n        y   
#>  here        y         n        y   
#>  highr       y         n        y   
#>  hms         y         n        y   
#>  htmltools   y         n        y   
#>  httr2       y         n        y   
#>  ini         y         n        y   
#>  jquerylib   y         n        y   
#>  jsonlite    y         n        y   
#>  knitr       y         n        y   
#>  lifecycle   y         n        y   
#>  magrittr    y         n        y   
#>  memoise     y         n        y   
#>  mime        y         n        y   
#>  openssl     y         n        y   
#>  pillar      y         n        y   
#>  pkgconfig   y         n        y   
#>  prettyunits y         n        y   
#>  progress    y         n        y   
#>  purrr       y         n        y   
#>  R6          y         n        y   
#>  rappdirs    y         n        y   
#>  readr       y         n        y   
#>  rlang       y         n        y   
#>  rmarkdown   y         n        y   
#>  rprojroot   y         n        y   
#>  rstudioapi  y         n        y   
#>  sass        y         n        y   
#>  stringi     y         n        y   
#>  stringr     y         n        y   
#>  sys         y         n        y   
#>  tibble      y         n        y   
#>  tidyr       y         n        y   
#>  tidyselect  y         n        y   
#>  tinytex     y         n        y   
#>  tzdb        y         n        y   
#>  usethis     y         n        y   
#>  utf8        y         n        y   
#>  vctrs       y         n        y   
#>  vroom       y         n        y   
#>  whisker     y         n        y   
#>  withr       y         n        y   
#>  xfun        y         n        y   
#>  yaml        y         n        y   
#>  zip         y         n        y   
#> 
#> The following package(s) are out of sync [lockfile != library]:
#> 
#> # CRAN -----------------------------------------------------------------------
#> - renv   [1.0.7 != 1.0.9]
#> 
#> See `]8;;ide:help:renv::status?renv::status]8;;` for advice on resolving these issues.
```

## Readme

``` r
usethis::use_readme_rmd()
#> ✔ Setting active project to "/Users/esingurcan/Desktop/GEO
#>   712/my-GEO712-repository/my-GEO712-repository".
#> ℹ Leaving 'README.Rmd' unchanged.
```

# My First Repo

<!-- badgers:start -->
<!-- badgers:end -->

This is my first repository. It contains several folders with assets. -
Folder `images` cıntains jpeg, bmp, and so on files that i need for my
documents. - Folder `plots` contains images that i generate through
code, pussibly for publisher.

The function `print()` will display the argument on the screen.

# First Assignment Content

# My Research Interest

My research focuses on understanding ***early markers*** and the
***genetic component of autism***. In these studies, we are
investigating;

- Early markers of autism in children with a familial history of autism,
  and
- Autism characteristics in family members of individuals with autism,
  focusing on the perceptual strengths associated with autism.

[Our lab website](https://pnb.mcmaster.ca/rutherford/)

# Favorites

## Favorite Music

1.  Hollow Coves - Home
2.  Gracie Abrams - I love you, I’m sorry
3.  Noah Kahan ft Hozier - Northern Attitude
4.  Noah Kahan - Everything, everywhere
5.  Zach Bryan - Pink skies

## Favorite Equation

$$
y =  \log_8(\frac{10}{8})
$$

## Favorite Artists

| Artist Name   | Achievements                                                                 |
|---------------|------------------------------------------------------------------------------|
| Noah Kahan    | Best New Artist iHeart Radio Music Awards, 2024                              |
| Gracie Abrams | Social Star Award iHeart Radio Music Awards, 2024 and Forbes 30 Under 30 2nd |
| Hollow Coves  | They did not win any awards but i love the stories behind their songs        |
| Taylor Swift  | She won 667 awards wow (according to wiki)                                   |
| Post Malone   | He won 30 awards including 10 Billboard Music Awards                         |

# A Chunk of Code

    model <- '
      # Direct paths
      Expressive_v ~ mouth_percent + aut_degree_cont + ADOS_Score + Gross_v 
      # Moderation path
      Expressive_v ~ mouth_percent*ADOS_Score
      Expressive_v ~ mouth_percent*aut_degree_cont
    '

    model_2 <- '
      # Direct paths
      Receptive_v ~ mouth_percent + aut_degree_cont + ADOS_Score + Gross_v 
      # Moderation path
      Receptive_v ~ mouth_percent*ADOS_Score
      Receptive_v ~ mouth_percent*aut_degree_cont
    '

    fit <- sem(model, data = data_12m) # For expressive
    summary(fit, fit.measures = TRUE, standardized = TRUE, rsquare = TRUE)

    fit_2 <- sem(model_2, data= data_12m) # For Receptive
    summary(fit_2, fit.measures = TRUE, standardized = TRUE, rsquare = TRUE)

## Git

This repository now is set up for git.

## Github

I also set up or I ’m working to set up a github repository.
