# Snakemake workflow: rna-seq-kallisto-sleuth

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4675671.svg)](https://doi.org/10.5281/zenodo.4675671)
[![Snakemake](https://img.shields.io/badge/snakemake-≥6.3.0-brightgreen.svg)](https://snakemake.github.io)
[![Snakemake-Report](https://img.shields.io/badge/snakemake-report-green.svg)](https://cdn.rawgit.com/snakemake-workflows/rna-seq-kallisto-sleuth/main/.test/report.html)

A Snakemake workflow for differential expression analysis of RNA-seq data with [Kallisto](https://pachterlab.github.io/kallisto) and [Sleuth](https://pachterlab.github.io/sleuth).

This version has been modified to include:
  - Kallisto genomebam functionality
  - Production of genomic .bam files using STAR alignment

## Usage

The usage of the original workflow is described in the [Snakemake Workflow Catalog](https://snakemake.github.io/snakemake-workflow-catalog/?usage=snakemake-workflows%2Frna-seq-kallisto-sleuth).

To use this modified workflow, follow the same steps as described in the link above except in step 2 for deploying the workflow. Using snakedeploy, run the following command instead:
<pre><code> snakedeploy deploy-workflow https://github.com/CCI-CDDB/rna-seq-kallisto-sleuthV2 . --branch main
</code></pre>
Once deployed, **please check that the local config.yaml file is the same as that found in this repository**. If this is not the case, please manually download the config file from this repository and use it instead in your locally created config directory. The additional functions can be toggled on or off from this config file.


If you use this workflow in a paper, don't forget to give credits to the (original) authors by citing the URL of the original repository and its DOI (see above).

