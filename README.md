# RMIT_MBP_SCworkshop_Oct2019
Links to resources from todays workshop.

Slides: https://github.com/MonashBioinformaticsPlatform/RMIT_MBP_SCworkshop_Oct2019/blob/master/RMIT-MBP-SCworkshop-22Oct19.pdf


In R, install the required packages with:

`install.packages(c("Seurat", "dplyr"))`

If you don't have Rmarkdown installed, install all of them with:

`install.packages(c("Seurat", "dplyr", "rmarkdown"))`


Download raw data here:

https://s3-us-west-2.amazonaws.com/10x.files/samples/cell/pbmc3k/pbmc3k_filtered_gene_bc_matrices.tar.gz

In your R-Studio, open a terminal window and use:

```
wget https://s3-us-west-2.amazonaws.com/10x.files/samples/cell/pbmc3k/pbmc3k_filtered_gene_bc_matrices.tar.gz
tar -xvf pbmc3k_filtered_gene_bc_matrices.tar.gz
```

Copy the workflow.Rmd file into the same directory as the pbmc3k_filtered_gene_bc_matrices. If need be, adjust `pbmc.data <- Read10X(data.dir = "filtered_gene_bc_matrices/hg19/")` to point to the correct directory location.

You should be able to knit the workflow file
