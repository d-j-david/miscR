# miscR

miscR is a collection of self-written functions to simplify some of my commonly performed tasks. 
They are designed to have exceptional user-friendliness.

## Usage

The following functions are contained in this package. A short description is given for each. For 
more detailed information, type `?functionName` into your R console after the package has been 
loaded. For instructions on how to load this package, read [Installation](#installation).

* [sample.df](#sampledf)
* [auth.connect](#authconnect)
* [time.log](#timelog)

### sample.df

Returns a random sample of a given data frame, either simple or stratified, depending on inputs. 

### auth.connect

Creates a connection to an external database that requires authentication, without having to write
credentials into the code itself. That connection, in turn, can be used in sqlQuery {RODBC} to query 
the database directly from R.

### time.log

Creates a background table for logging and reading times. This can be useful for calculating the run
time of code, or particularly, for helping to estimate the time remaining in an iterative process.

## Installation

This package can be accessed directly from R, without any additional coercion. Simply copy and 
paste the following commands into your R console and run:

```
install.packages("devtools")  
devtools::install_github("d-j-david/miscR")  
library(miscR)
```

`install.packages("devtools")`, as you might guess, installs the [devtools package](https://github.com/hadley/devtools). 
`install_github` is a function within devtools which allows the user to install R packages directly 
from Github. `library(miscR)` actually loads the miscR package for the current instance, giving 
access to all the functions it contains.

After the initial install, only `library(miscR)` is needed to access the package in a given R 
instance, although it is a good idea to periodically run `devtools::install_github("d-j-david/miscR")` 
to keep the package up to date with the most current version.
