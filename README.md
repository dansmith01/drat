https://stackoverflow.com/a/64927507/3259270
https://stackoverflow.com/a/66852164/3259270

https://cran.r-project.org/web/packages/drat/vignettes/DratStepByStep.html

git clone https://github.com/coolbutuseless/ggpattern.git
cd ggpattern
R CMD build . --no-build-vignettes

library(drat)
options(dratBranch="docs")
insertPackage(file="ggpattern/ggpattern_0.2.0.tar.gz", repodir=".")
