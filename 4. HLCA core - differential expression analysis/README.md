## Differential expression analysis
This was run in R, on the Delft AI cluster (https://doc.daic.tudelft.nl). Scripts 1. and 2. cover the pre-processing, aggregation to pseudobulk and differential state analysis. The output is the final_DS_results dataframe, which contains the number and proportion of differentially expressed genes per cell type. The results for each individual cell type are also given in the individualDS folder, as .rds files. <br>

Notebook 3. combines the final_DS_results with the classification trends obtained in the previous section. It also makes use of the cell_type_info dictionary obtained after the epxloration in section 1. <br>

<br>

The workflow for the differential state analysis is adapted from the analysis vignette for the Bioconductor package muscat: <br>

Crowell, H. L., Stoneson C., Germain P.-L., Robinson, M. D. (2024). Differential state analysis with muscat. Bioconductor. https://www.bioconductor.org/packages/devel/bioc/vignettes/muscat/inst/doc/analysis.html <br>
