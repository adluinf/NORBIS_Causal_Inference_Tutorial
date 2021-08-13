# NORBIS Causal Inference Tutorial
##  2021.6.18

# Overview

This is a tutorial about **causal inference for genomics data** for the NORBIS Research School Course Genomics for Precision Medicine.

In this tutorial, you will look at a few TF/gene pairs from data published in [1]:

  - to study the ***distributions*** of expression values,
  - to perform ***linear regression*** to estimate **causal** effects,
  - to compare with results obtained with the **causal** ***Findr tests*** [2,3],
  - and to check on **databases** what the known interactions are.

**Note**: the Jupiter notebooks (files with ``.ipynb`` extension) can be run either locally if you have python and Jupyter installed on your system or you can load them in google [Colab](https://colab.research.google.com/notebooks/intro.ipynb).

# Covariates

The notebook ``Covariates_notebook.ipynb`` is setup to download the covariates file (``SI_Data_02_covariates.xlsx``) and generate a graphical representation of these covariates for the differential gene expression data from [1].

# Causal Tests with Linear Regression on Yeast Data

The notebook ``Causal_Inference_with_Linear_Regression_20210618.ipynb`` is setup to download the data files of differential gene expression data corrected for covariates. After that **you will preform the following tasks**:

  1. Make a **visualisation** of gene expression values.
  2. Perform **linear regression** on gene pairs and visualise the result.
  3. Answer the following question: "Are the distributions of the Regulator and Target Genes' expression values different for the possible Marker (eQTL) genotypes?"
  4. Check on **databases** what the known interactions are:
     * Yeastract:	http://www.yeastract.com
     * SGD:		https://www.yeastgenome.org
     * Ensembl:	https://fungi.ensembl.org/Saccharomyces_cerevisiae/Info/Index

# Additional files

There are two more files in this repository:

 - ``Example_1_covariate_regression_on_expression_data.py``: is a python script that does the covariate correction.

 - ``Example_2_yeast_run_findr.py``: allows you to run the Findr tests on the differential gene expression data. For more information about Findr see [3].

# References:

1. Albert et al. (2018) eLife, 7, e35471. *Genetics of trans-regulatory variation in gene expression*. [DOI](https://doi.org/10.7554/eLife.35471)

2. Ludl & Michoel. (2021) Molecular Omics, 17, 241-251. *Comparison between instrumental variable and mediation-based methods for reconstructing causal gene networks in yeast*. [DOI](https://doi.org/10.1039/D0MO00140F) -- [github repo](https://github.com/lingfeiwang/findr)

3. Wang & Michoel. (2017) PLOS Computational Biology, 13(8), e1005703. *Efficient and accurate causal inference with hidden confounders from genome-transcriptome variation data*. [DOI](https://doi.org/10.1371/journal.pcbi.1005703) -- [github repo](https://github.com/michoel-lab/FindrCausalNetworkInferenceOnYeast)
