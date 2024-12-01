# [An R package `PI4Medicine`](https://github.com/23verse/PI4Medicine)

## @ Overview

> The `PI4Medicine` is an R package introducing protocol for the software suite centering on Pi.

## @ Installation

### 1. Install R

Please install R (version 4.3.0 or above); see https://cran.r-project.org

If installed on `Ubuntu` (assuming you have a `ROOT (sudo)` privilege), please do so below

```ruby
sudo su
# here enter your password

wget http://www.stats.bris.ac.uk/R/src/base/R-4/R-4.3.0.tar.gz
tar xvfz R-4.3.0.tar.gz
cd ~/R-4.3.0
./configure
make
make check
make install
R # start R
```

### 2. Install R packages

```ruby
R # start R

# if the package 'BiocManager' not installed, please do so
if(!("BiocManager" %in% rownames(installed.packages()))) install.packages("BiocManager")

# first, install basic packages: remotes, tidyverse
BiocManager::install(c('remotes','tidyverse'), dependencies=T)

# then, install the package 'PI4Medicine' (now hosted at github)
BiocManager::install("23verse/PI4Medicine", dependencies=T, force=T)

# check the package 'PI4Medicine' successfully installed
library(help=PI4Medicine)
```


## @ Contact

> Please drop [email](mailto:fh12355@rjh.com.cn) for bug reports or other enquiries.


