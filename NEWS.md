NEWS
====

Shuowen Chen, Sebastián Gómez-Roca
10/06/2026

# SortedEffects 2.0.

Changes from SortedEffects 1.6.0. The package had been taken down from R because it used the now deprecated package [dummies](https://CRAN.R-project.org/package=dummies) (Brown, 2009, version 1.03). The dummy() and dummy.data.frame() functions are adapted from Christopher Brown's original package, with only some minor changes. They were included after the package dummies was removed from CRAN, with permission from the original author, to whom we are thankful and that is why he appears as one of the contributors of the project. Additionally, arguments for the `plot` function are now named to avoid inconsistencies in case of updates to this function.

Changes from SortedEffects 1.5.0. The previous version imports a package rlist. Upon receving a warning from CRAN about reverse dependencies, we revise the code so that the package no longer relies on rlist.

Changes from SortedEffects 1.4.0. Renormalize the weights for stable estimates using glm.

Changes from SortedEffects 1.3.0. For nonparametric bootstrap, we use the multinomial weight resampling to produce more stable bootstrap estimates.

Changes from SortedEffects 1.2.0. The spe function in the 1.2.0 version produces far wider nonparametric bootstrap confidence bands for some specifications. We fix that issue.

Changes from SortedEffects 1.1.0. The 1.1.0 version has a check problem due to a recent upgrade of package 'tibble' to version 3.0. The package doesn't really need tibble package, so we change the data type.
