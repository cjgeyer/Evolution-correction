This git repo holds the files for the supplementary material for a
correction to the paper

> Mason W. Kulbaba, Seema N. Sheth, Rachel E. Pain, Vincent M. Eckhart and Ruth G. Shaw (2019).  
> Additive genetic variance for lifetime fitness and the capacity for adaptation in an annual plant.  
> *Evolution* 73:1746–1758.  
> doi: [10.1111/evo.13830](https://doi.org/10.1111/evo.13830).

The correction has already been accepted by *Evolution* and has manuscript
number 22-0427.

The supplementary material is the PDF file
[vaw.pdf](https://github.com/cjgeyer/Evolution-correction/blob/main/vaw.pdf)
in this repo.

This file is fully reproducible, to reproduce it download the repo and do

    Rscript -e 'rmarkdown::render("vaw.Rmd")'

at the operating system command line to make

    vaw.pdf

which is the supplementary material for the correction.

This takes several hours to run, but caches results so that runs after
that take less than a minute.

Needs R and CRAN packages

    rmarkdown
    bookdown
    aster
    numDeriv
    kableExtra

In R

    install.packages(c("bookdown", "aster", "numDeriv", "kableExtra"))

will install these packages.

Also needs the files

    csdata.csv
    gcdata.csv
    kwdata.csv
    foo.bib
    journal-of-the-royal-statistical-society.csl

(which are needed to render the Rmarkdown and are in this git repo).

The csv files are the data for the original paper, which has not changed
for this correction.  Only the analysis in the Rmarkdown file differs.
