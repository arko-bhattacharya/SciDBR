[![CRAN version](http://www.r-pkg.org/badges/version/irlba)](http://cran.rstudio.com/web/packages/scidb/index.html)
![](http://cranlogs.r-pkg.org/badges/scidb)
[![codecov.io](https://codecov.io/github/paradigm4/scidbr/coverage.svg?branch=laboratory)](https://codecov.io/github/paradigm4/scidbr?branch=laboratory)

Install the package from CRAN with
```
install.packages("scidb")
```

The current development version of the package can be installed directly from
sources on  GitHub using the devtools package as follows (requires an R
development environment  and the R devtools package):
```
devtools::install_github("Paradigm4/SciDBR")
```

The SciDB R package requires installation of a simple open-source HTTP network
service called on the computer that SciDB is installed on. This service only
needs to be installed on the SciDB machine, not on client computers that
connect to SciDB from R.  See http://github.com/paradigm4/shim  for source code
and installation instructions.

Developers please note that R CMD check-style unit tests are skipped unless a
system environment variable named SCIDB\_TEST\_HOST is set to the host name or
I.P. address of SciDB. See the tests directory for test code.

## Wiki
Check out (and feel free to contribute to) examples in the wiki pages for
this project here:

https://github.com/Paradigm4/SciDBR/wiki/_pages

## Getting Started Documentation

https://Paradigm4.github.io/SciDBR


## Changes in package version 2.0.0

This is a major release that breaks API compatibility with previous package
releases.  Array objects have been removed. All SciDB arrays are now presented
as virtual data frames in R. This change was informed by the most common uses
we've seen.

