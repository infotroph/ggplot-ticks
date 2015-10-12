ggplotTicks
============

Put scale ticks on all four sides on a ggplot by copying axes from bottom to top and left to right.


Think of this as a replacement for the panel grid, not a way of adding multiple scales to the same plot.

Note that this function converts the plot from a ggplot object to a gtable,
so build the whole plot first and then call mirror-ticks as the last transformation before plotting.

## Installation:

### From R using `devtools` (recommended)
```
install.packages("devtools")
library("devtools")
install_github("infotroph/ggplotTicks")
```
Note that I *think* you can ignore the step of the `devtools` [installation instructions](https://cran.r-project.org/web/packages/devtools/README.html) where it claims you need a full development toolchain (on OS X this involves a multi-gigabyte download of Xcode). If you have any trouble installing on a machine with no developer tools, please let me know.

### From a command line

Modify this as needed for your system. Probably only necessary if you want to edit the package code.
```
git clone https://github.com/infotroph/ggplotTicks.git
R CMD build ggplotTicks
R CMD install ggplotTicks_<version.number.here>.tar.gz
```

Once installed, load and use it like any other package: `library(ggplotTicks); myplot = ggplot(...); mirror.ticks(myplot)`
