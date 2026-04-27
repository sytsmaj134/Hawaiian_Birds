# Hawaiian Birds Genomics Analysis

## Overview

This repository contains code and data for analyzing genomic diversity and population trends in Hawaiian birds. The project integrates whole-genome sequencing data with occurrence-based metrics to assess patterns of genetic variation, inbreeding, and population health across species with contrasting conservation status.

By combining ecological and genomic data, this workflow provides a reproducible framework for detecting genomic erosion associated with population decline and for evaluating conservation risk in island ecosystems.

---

## Objectives

This project addresses three primary questions:

1. How do occurrence trends vary among Hawaiian bird species?
2. How does genomic diversity differ across species with contrasting demographic histories?
3. Are declines in occurrence associated with reduced genomic diversity and increased inbreeding?

---

## Study System

The dataset includes four Hawaiian bird species representing a gradient of conservation status:

- **Hawaiʻi ʻamakihi** (*Chlorodrepanis virens*)
- **ʻAlalā** (*Corvus hawaiiensis*)
- **Maui parrotbill** (*Pseudonestor xanthophrys*)
- **Christmas shearwater** (*Puffinus nativitatis*)

---

## Data

The repository uses a practice dataset simulating outputs from whole-genome sequencing analyses.

### Included data:
- Individual-level genomic metrics:
  - nucleotide diversity (π)
  - heterozygosity
  - runs of homozygosity (ROH)
  - inbreeding coefficient (F)
- PCA coordinates (genomic variation)
- Site frequency spectrum (SFS)


---

## Analysis Workflow

The R script performs the following steps:

### 1. Data Processing
- Imports genomic datasets
- Cleans and standardizes species labels

### 2. Summary Statistics
- Calculates species-level means and standard deviations
- Produces publication-ready summary tables

### 3. Statistical Analysis
- ANOVA tests across species
- Tukey post hoc comparisons
- Correlation analyses between genomic variables

### 4. Visualization
- Violin + boxplots for:
  - nucleotide diversity
  - heterozygosity
  - ROH
  - inbreeding
- PCA plots of genomic variation
- Site frequency spectrum plots
- Scatterplots of genomic relationships

### 5. Genomic Risk Index
- Combines standardized genomic metrics into a composite risk score
- Ranks species by genomic vulnerability

Outputs
Figures
Genetic diversity distributions
PCA of genomic variation
Site frequency spectrum plots
Genomic risk index
Tables
Species-level summary statistics
Publication-ready tables
Genomic risk index values
Statistical Results
ANOVA outputs
Post hoc tests
Correlation tests
Dependencies

R packages used:

readxl
dplyr
tidyr
ggplot2
forcats
scales
stringr
Reproducibility

All analyses are fully reproducible using the provided script and dataset.
Outputs are generated programmatically and saved automatically.

Notes
This dataset is simulated for practice and demonstration purposes.
The workflow is designed to reflect realistic conservation genomics analyses.
The code structure can be adapted to real whole-genome sequencing datasets.
Future Directions

Potential extensions include:

STRUCTURE / admixture analysis
Demographic modeling (e.g., ∂a∂i, MSMC)
Selection scans
Integration with spatial/environmental data
Island-level population structure analysis
Author
Jack Sytsma
Kansas State University
sytsmaj134@ksu.edu
