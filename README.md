# glm-hicexp #

Obtain differentially interacting regions using glm methods to test a normalized hicexp object

## input ##

A normalized hicexp object. The input hicexp may contain samples of 2 OR of 3 different groups. The `glm-normalized-hicexp.R` script should be softlinked accordingly.



### Requirements ###

- [`mk`](http://doc.cat-v.org/bell_labs/mk/mk.pdf "A successor for `make`.")

- [`multiHiCCompare`](https://github.com/dozmorovlab/multiHiCcompare)

- [`BiocParallel`](https://bioconductor.org/packages/release/bioc/html/BiocParallel.html)

- [`optparse`](https://cran.r-project.org/web/packages/optparse/index.html)


### Note ###

This module does not include the filtering of results to obtain significant differentially interacting regions (DIRs)... perhaps this could be an issue if there's too little memory available since the output in this case is a list of hicexp objects that can be heavy. I might consider creating a light module where the same hicexp object is reused and only results are written out as plain text.


