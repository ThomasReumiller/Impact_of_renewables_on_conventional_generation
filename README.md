This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

The paper the problem set is based on examines the effects increasing renewable energy output has on conventional generation, prices and emissions. The paper itself can be downloaded here:
https://www.journals.uchicago.edu/doi/abs/10.1086/713249
and the data is available here:
https://doi.org/10.7910/DVN/6XQZ3L

In case you do not want to install the problem set, you may have a look here: https://thomasreumiller.shinyapps.io/Impact_of_renewables_on_conventional_generation/.
However, you are not able to store your progress there.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("ThomasReumiller/RTutorImpactOfRenewablesOnConventionalGeneration")
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorImpactOfRenewablesOnConventionalGeneration)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorImpactOfRenewablesOnConventionalGeneration")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorImpactOfRenewablesOnConventionalGeneration",
       auto.save.code=TRUE, clear.user=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
