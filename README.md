# Assessing the effects of sex bias on cell type classification in scRNA-seq data

## Organization
This repository is divided into 9 sub-sections of experiments.

* On the HLCA core:
  - Exploration
  - Classification templates
  - Analysis of classification results
  - Differential expression analysis

* For the disease data:
  - Generation + Exploration
  - Classification templates
  - Analysis of classification results
  - Differential expression analysis (for COVID-19 only)

* Batch correction for a subset of the HLCA core.


Sub-sections are numbered in the order that they are being referred to in the paper; notebooks or scripts within each folder are also numbered. Several analyses require results from previous experiments to work, thus everything should be run in order when repeating. Most experiments are performed  in Jupyter notebooks, but a few use Python or R scripts. Paths to import the data or results from other analyses should be changed when re-running the code.

For the classification experiment, the full code is not given as it consists of hundreds of near-identical scripts. Instead, a sample script is included for every experiment, along with instructions on how to generate subsequent scripts. The classification results are given in full.

## Data availability
This research uses data from the Human Lung Cell Atlas (Sikkema et al., 2023). The data can be downloaded from the CELLxGENE database: https://cellxgene.cziscience.com/collections/6f6d381a-7701-4781-935c-db10d30de293. 

The data is used in both the .h5ad format (for the analyses in Python) and in the Seurat format (for those in R). Specifically:
- analyses in folders 1., 2., 3., 5., 6., 7., 9. only use the .h5ad data
- analyses in folders 4. and 8. use the Seurat object (or both the Seurat and the .h5ad object)
