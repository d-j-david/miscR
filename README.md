# miscR

miscR is a collection of self-written functions to simplify some of my commonly performed tasks. 
They are designed to have exceptional user-friendliness.

## Usage

The following functions are contained in this package. A short description is given for each. For 
more detailed information, type `?functionName` into your R console after the package has been 
loaded. For instructions on how to load this package, read [Installation](#Installation).

* [sample.df](###sample.df)
* [auth.connect](###auth.connect)
* [time.log](###time.log)

### sample.df

Returns a random sample of a given data frame, either simple or stratified, depending on inputs. 

### auth.connect

Creates connection to an external database that requires authentication, without having to write
credentials into the code itself. That connection, in turn, can be used in sqlQuery to query the
database directly from R.

### time.log

Creates a background table for logging and reading times. This can be useful for calculating the run
time of code, or particularly, for helping to estimate the time remaining in an iterative process.

## Installation

This package can be accessed directly from R, without any additional coercion. Simply copy and 
paste the following commands into your R console and run:

```R
install.packages("devtools")  
devtools::install_github("d-j-david/miscR")  
library(miscR)
```

This code installs the [devtools package](https://github.com/hadley/devtools), containing the 
function `install_github`, which allows you to install R packages directly from Github. Once miscR 
is installed on your machine, running `library(miscR)` will load the package for your current 
instance, giving access to all the functions it contains.
