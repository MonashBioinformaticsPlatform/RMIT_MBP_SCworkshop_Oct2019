# RMIT_MBP_SCworkshop_Oct2019
Links to resources from todays workshop.

Slides: https://github.com/MonashBioinformaticsPlatform/RMIT_MBP_SCworkshop_Oct2019/blob/master/RMIT-MBP-SCworkshop-22Oct19.pdf


If you don't have R-Studio and R installed, you can use RStudio Cloud:

https://rstudio.cloud

In R, install the required packages with:

```
install.packages(c("Seurat", "dplyr", "reticulate"))
reticulate::py_install(packages = "umap-learn")
```

If you don't have Rmarkdown installed, install all of them with:

`install.packages(c("Seurat", "dplyr", "reticulate", "rmarkdown"))`


Download raw data here:

https://s3-us-west-2.amazonaws.com/10x.files/samples/cell/pbmc3k/pbmc3k_filtered_gene_bc_matrices.tar.gz

In your R-Studio, open a terminal window and use:

```
wget https://s3-us-west-2.amazonaws.com/10x.files/samples/cell/pbmc3k/pbmc3k_filtered_gene_bc_matrices.tar.gz
tar -xvf pbmc3k_filtered_gene_bc_matrices.tar.gz
```

Copy the seurat_workflow.Rmd file into the same directory as the pbmc3k_filtered_gene_bc_matrices. This workflow can also be found: https://satijalab.org/seurat/v3.1/pbmc3k_tutorial.html

If need be, adjust `pbmc.data <- Read10X(data.dir = "filtered_gene_bc_matrices/hg19/")` to point to the correct directory location. 

You should be able to knit the workflow file
