# NORBIS Causal Inference Tutorial
##  2021.6.18

This is a tutorial about **causal inference for genomics data** for the NORBIS Research School Course Genomics for Precision Medicine.

In this tutorial, you will look at a few TF/gene pairs from data published in [1]:

  - to study the *distributions* of expression values,
  - to perform *linear regression* to estimate **causal** effects,
  - to compare with results obtained with the **causal** *Findr tests* [2],
  - and to check on **databases** what the known interactions are:
    * Yeastract:	http://www.yeastract.com
    * SGD:		https://www.yeastgenome.org
    * Ensembl:	https://fungi.ensembl.org/Saccharomyces_cerevisiae/Info/Index

# Covariates

The notebook ``Covariates_notebook.ipynb`` is setup to download the covariates file (``SI_Data_02_covariates.xlsx``) and generate a graphical representation of these covariates for the differential gene expression data from [1].

# Causal Tests with Linear Regression on Yeast Data

The notebook ``Causal_Inference_with_Linear_Regression_20210618.ipynb`` is setup to download the data files of differential gene expression data corrected for covariates. After that **you will preform the following tasks**:

  1. Make a *visualisation* of gene expression values.
  2. Perform *linear regression* on gene pairs and visualise the result.
  3. Answer the following question: "Are the distributions of the Regulator and Target Genes' expression values different for the possible Marker (eQTL) genotypes?"

# References:

1. Albert et al. (2018) eLife, 7, e35471. *Genetics of trans-regulatory variation in gene expression*. [DOI](https://doi.org/10.7554/eLife.35471)

2. Ludl & Michoel (2021) Mol. Omics, 17, 241-251. *Comparison between instrumental variable and mediation-based methods for reconstructing causal gene networks in yeast*. [DOI](https://doi.org/10.1039/D0MO00140F)
