# Experimental defaunation modifies diet and gut microbiome of a wild gerbil, *Gerbilliscus robustus*

**Bianca R. P. Brown, Leo M. Khasoha, Todd M. Palmer, Robert M. Pringle, Seth D. Newsome, Jacob R. Goheen, Tyler R. Kartzinel**

---

## Overview

This repository contains the R scripts and workflows used to reproduce all analyses in the manuscript  
*Experimental defaunation modifies diet and gut microbiome of a wild gerbil, Gerbilliscus robustus*.  
Scripts are organized to match the analytical components presented in the figures and results.

All required files will be made publicly available on Zenodo:
https://doi.org/10.5281/zenodo.17743788

---


## 1. Vegetation analysis  
**File:** `01.Vegetation.Rmd`

Scripts and data for tree census estimates, vegetation structure, and treatment-level comparisons.

**Dependencies:**  
tidyverse, readr, vegan, ape, lme4, lmerTest, emmeans, rstatix, ggpubr

---

## 2. Isotope diet analysis  
**File:** `02.Isotopediet.Rmd`

Diet estimation using the `rKIN` package, including δ¹³C and δ¹⁵N data preparation, isotopic niche calculations, and seasonal comparisons.

**Dependencies:**  
rKIN, tidyverse, ggplot2

---

## 3. Microbiome diversity and composition  
**File:** `03.MicrobiomeDiversityAnalysis.Rmd`

Preprocessing, ordination, α- and β-diversity calculations, PERMANOVA, and taxonomic summaries.

**Dependencies:**  
phyloseq, microbiome, mia, ggplot2, dplyr, vegan

---

## 4. Differential abundance analysis (ANCOM-BC)  
**File:** `04.Differentialabundance.Rmd`

Differential abundance testing across treatments and locations using ANCOM-BC, including preprocessing, model fitting, and extraction of significant taxa.

**Dependencies:**  
phyloseq, microbiome, mia, ANCOMBC, ggpubr, dplyr, ggplot2

---

## Reproducibility

Permutation-based analyses (e.g., PERMANOVA, Mantel tests) include explicit `set.seed()` statements to ensure reproducibility.  
All scripts are annotated and aligned with the analytical steps described in the manuscript.

---

## Data availability

Data for vegetation, isotope analyses, and microbiome sequencing are structured by analysis section and will be made available upon publication.

Illumina 16S rRNA data are publicly available at the National Center for Biotechnology Information (NCBI) Sequence Read Archive (SRA):

**BioProject:** [PRJNA961814](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA961814)

---

## Citation

If you use material from this repository, please cite:

**Brown et al.**, *Experimental defaunation modifies diet and gut microbiome of a wild gerbil, Gerbilliscus robustus* (in review).

Questions
Email: biancarpalmerbrown@gmail.com

