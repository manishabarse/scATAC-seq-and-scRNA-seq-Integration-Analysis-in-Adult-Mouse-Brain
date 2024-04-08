# scATAC-seq and scRNA-seq Integration Analysis in Adult Mouse Brain

## Overview
This repository contains the code and data for integrating and analyzing single-cell RNA sequencing (scRNA-seq) and single-cell ATAC sequencing (scATAC-seq) data from the adult mouse brain. The analysis pipeline is implemented in R and utilizes the `Seurat` and `Signac` packages for processing and integration.

## Aim
The primary goal of this project was to learn and understand the integration of scATAC-seq and scRNA-seq data, along with the utilization of the `Signac` and `Seurat` packages. By following the tutorial provided in the [Signac GitHub repository](https://github.com/stuart-lab/signac/blob/master/vignettes/mouse_brain_vignette.Rmd), I aimed to gain practical experience in bioinformatics pipeline development, data integration, and analysis.

## Data Sources
The scATAC-seq and scRNA-seq data used in this analysis were obtained from the 10x Genomics website:
- scATAC-seq data:
  - Peak matrix: [atac_v1_adult_brain_fresh_5k_filtered_peak_bc_matrix.h5](http://cf.10xgenomics.com/samples/cell-atac/1.1.0/atac_v1_adult_brain_fresh_5k/atac_v1_adult_brain_fresh_5k_filtered_peak_bc_matrix.h5)
  - Cell metadata: [atac_v1_adult_brain_fresh_5k_singlecell.csv](http://cf.10xgenomics.com/samples/cell-atac/1.1.0/atac_v1_adult_brain_fresh_5k/atac_v1_adult_brain_fresh_5k_singlecell.csv)
  - Fragments file: [atac_v1_adult_brain_fresh_5k_fragments.tsv.gz](http://cf.10xgenomics.com/samples/cell-atac/1.1.0/atac_v1_adult_brain_fresh_5k/atac_v1_adult_brain_fresh_5k_fragments.tsv.gz)
  - Index file [atac_v1_adult_brain_fresh_5k_fragments.tsv.gz.tbi](http://cf.10xgenomics.com/samples/cell-atac/1.1.0/atac_v1_adult_brain_fresh_5k/atac_v1_adult_brain_fresh_5k_fragments.tsv.gz.tbi)
- scRNA-seq data:
  - Raw data: [Allen Institute](http://celltypes.brain-map.org/api/v2/well_known_file_download/694413985)
  - Pre-processed Seurat object: [allen-brain-RDS](https://signac-objects.s3.amazonaws.com/allen_brain.rds)

## Repository Contents
- **scatac-seq-adult-mouse-brain.Rmd**: This R Markdown file contains the code for the integration and analysis of scRNA-seq and scATAC-seq data.
- **scatac-seq-adult-mouse-brain.html**: The rendered HTML output of the analysis script.
- **README.md**: This README file providing an overview of the project, its aim, data sources, and repository contents.

## Requirements
- R version: 4.3.3
- R packages:
  - `Seurat`
  - `Signac`
  - Other required packages as specified in the analysis script.

## Usage
To reproduce the analysis:
1. Clone or download this repository.
2. Ensure that the required data files are placed in the appropriate directory.
3. Open and run the `analysis_script.Rmd` file in RStudio or any other compatible environment.
4. Follow the instructions provided in the analysis script to execute the analysis steps.

## Acknowledgments
- The Stuart Lab for providing the tutorial on scATAC-seq and scRNA-seq integration using the `Signac` package.
- 10x Genomics for providing the scATAC-seq data used in this analysis.
