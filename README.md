# R-Programming-III


To aid her in this effort, you are expected to provide a vignette which outlines how the package works. See a completed example [here](https://bioinformatics-research-network.github.io/R-Programming-II/bioutils_quickstart.html).

The easiest way to create one is the run:

```R
usethis::use_vignette(name = "bioutils_quickstart", title = "BioUtils Quickstart")
```

This will create an [RMarkdown](https://rmarkdown.rstudio.com/) document, `vignettes/bioutils_quickstart.Rmd`. Edit this document to create your vignette. 

Then, build your vignette like so:

```R
devtools::build_vignettes()
```

This will create an HTML document in the following location: `doc/bioutils_quickstart.html`. This is the HTML (user-friendly) vignette.

Finally, it will ensure that your vignette(s) can be successfully built from the linux command line (test this in R by running `devtools::build_vignettes()`):

```shell
Rscript -e "if (is.null(devtools::build_vignettes())) quit(save = 'no', status = 1)"
```
