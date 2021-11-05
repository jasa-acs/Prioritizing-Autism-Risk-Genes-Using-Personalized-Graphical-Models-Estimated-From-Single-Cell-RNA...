# Prioritizing Autism Risk Genes Using Personalized Graphical Models Estimated From Single-Cell RNA-seq Data
### Jianyu Liu, Haodong Wang, Wei Sun & Yufeng Liu
# Author Contributions Checklist Form

## Data

**Abstract (Mandatory)**

We have used two datasets to evaluate our method. The first one is the single nuclei sequencing dataset from brain samples of 13 autism patients and 10 controls (Velmeshev D et al. 2019, Science, 364(6441): 685-689.). The number of cells varies from less than 100 to more than 1000 per individual and we chose to study those individuals with a larger number of cells to ensure there are enough samples (the number of cells) to study gene-gene interactions. The second one measures the expression of 24,187 genes in 1,500 human macrophage cells of the HEK293 cell line (Gierahn T M et al. 2017, Nature methods, 14(4): 395-398.). The cells are profiled with the Seq-Well technique, which is similar to the droplet technique and also uses UMIs.

**Availability (Mandatory)**

All datasets used in the paper are publicly available.

Dataset of Gierahn et al.

It was downloaded from [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE9249](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE9249). The dataset we used were extracted from &quot;GSM2486331\_HEK\_SingleCells.txt&quot; in the file &quot;GSE92495\_RAW.tar&quot;. The import code is included in GitHub as follows: [https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd](https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd)

Dataset of Velmeshev et al.

It was downloaded from [https://cells.ucsc.edu/autism/rawMatrix.zip](https://cells.ucsc.edu/autism/rawMatrix.zip). The import code is included in GitHub: [https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd](https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd).

**Description (Mandatory if data available)**

We have included the data needed to reproduce our results as well as our code in GitHub: [https://github.com/hwang655/HUG/tree/master/data](https://github.com/hwang655/HUG/tree/master/data)

We also include a sample code to generate simulated data:

[https://github.com/hwang655/HUG/tree/master/example](https://github.com/hwang655/HUG/tree/master/example)

**Optional Information (complete as necessary)**

Unique identifier / DOI

## Code

**Abstract (Mandatory)**

We have implemented our method as a R package HUG.

**Description (Mandatory)**

The R package as well as detailed readme file are available at [https://github.com/hwang655/HUG/](https://github.com/hwang655/HUG/)

In addition, we have made all the codes needed available to reproduce our real data analyses results and simulation studies. The versions of all relevant R packages are listed below.

attached base packages:

[1] grid parallel stats graphics grDevices utils

[7] datasets methods base

other attached packages:

[1] MASS\_7.3-51.5 HUG\_1.3 doSNOW\_1.0.19

[4] snow\_0.4-3 igraph\_1.2.6 huge\_1.3.4.1

[7] glmnet\_4.1 mvtnorm\_1.1-1 fields\_11.6

[10] spam\_2.6-0 dotCall64\_1.0-0 qlcMatrix\_0.9.7

[13] sparsesvd\_0.2 slam\_0.1-48 doParallel\_1.0.16

[16] iterators\_1.0.13 foreach\_1.5.1 Matrix\_1.2-18

loaded via a namespace (and not attached):

[1] Rcpp\_1.0.6 rstudioapi\_0.11 magrittr\_2.0.1

[4] maps\_3.3.0 splines\_3.6.3 docopt\_0.7.1

[7] lattice\_0.20-38 fansi\_0.4.1 tools\_3.6.3

[10] sessioninfo\_1.1.1 cli\_2.0.2 withr\_2.1.2

[13] assertthat\_0.2.1 survival\_3.1-8 crayon\_1.3.4

[16] codetools\_0.2-16 glue\_1.4.0 shape\_1.4.5

[19] compiler\_3.6.3 pkgconfig\_2.0.3

**Optional Information (complete as necessary)**

## Instructions for Use

**Reproducibility (Mandatory)**

All the results of our analyses can be reproduced. The real data analyses of Velmeshev et.al take multiple steps because we have started from raw data. We loaded the data using function read10xCounts from R package DropletUtils. The import and preprocess programs are included in GitHub: [https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd](https://github.com/hwang655/HUG/blob/master/scripts/ImportData.Rmd). We have also provided the R code to reproduce the results in our GitHub websites using processed data. The README file at [https://github.com/hwang655/HUG/](https://github.com/hwang655/HUG/) provides an example to run ICeDT. The simulation code is located at [https://github.com/hwang655/HUG/tree/master/example](https://github.com/hwang655/HUG/tree/master/example). The real data analysis code is located at [https://github.com/hwang655/HUG/tree/master/simulations](https://github.com/hwang655/HUG/tree/master/simulations).

**Replication (Optional)**

The R package as well as detailed readme file is available at [https://github.com/hwang655/HUG/](https://github.com/hwang655/HUG/)
