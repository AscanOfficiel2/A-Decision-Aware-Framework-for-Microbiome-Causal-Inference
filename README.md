# Decision-Aware Framework for Microbiome Causal Inference

This repository accompanies the publication:
Ascandari A, Aminu S, Benhida R, Daoud R. (2026). From Association to Causation: A Decision-Aware Framework for Reproducible Biomarker Discovery and Precision Intervention Design in the Human Gut Microbiome. Briefings in Bioinformatics, 27(3), bbag316. It includes detailed results and figures generated from eight public colorectal cancer (CRC) metagenomic datasets available from the NCBI Sequence Read Archive (SRA) under accessions: PRJDB4176, PRJEB72525, PRJEB72526, PRJEB27928, PRJEB6070, PRJEB7774, and PRJNA1167935. The analysis applies:

- Data harmonization and CLR transformation
- DML estimation with cross-fitting (EconML)
- Bootstrap resampling (300 iterations)
- Negative control validation (*Acidaminococcus intestini*)
- E-value sensitivity analysis

## Framework Overview
The Decision-Aware Framework integrates causal assumption mapping, causal identification, effect estimation, and mechanistic validation into a structured workflow for microbiome research.

It combines DAGs, Mendelian randomization, longitudinal evidence, double machine learning (DML), and mediation analysis, with explicit assumption guardrails to ensure causal interpretations reflect the available evidence.
- The code for the DAG construction in dagitty
- The detailed statistical results can be found in the DML_bootstrap_negative_control_results.xlsx. 
- The figure of the DAG (saved as model.png)
- The forest plot with the negative control
- Bootstrap distributions

## CRC Demonstration

This repository provides the scripts, supporting data, statistical results, and figures for the illustrative CRC analysis presented in the publication.
The demonstration used 995 samples from seven public CRC cohorts to investigate the association between Fusobacterium nucleatum and CRC under limited-data conditions.
The analysis included:
- Data harmonization, CLR transformation and batch correction.
- DAG-based assumption mapping using Dagitty.
- DML estimation with five-fold cross-fitting (EconML).
- Bootstrap validation (300 iterations).
- Negative-control analysis using Acidaminococcus intestini.
- E-value sensitivity analysis.

### Main finding: F. nucleatum showed a positive adjusted association with CRC (estimate = 0.026; 95% CI: 0.021–0.032). However, causal directionality could not be established because longitudinal and host genetic evidence were unavailable.

## Repository Outputs

Scripts and supporting analytical data for the CRC demonstration.

- DAG specification and figure (model.png).
- Statistical results (DML_bootstrap_negative_control_results.xlsx).
- DML forest plot and bootstrap distributions.

## Citation
When applying the code or using the results in this repository, please cite:

Ascandari A, Aminu S, Benhida R, Daoud R. (2026). From Association to Causation: A Decision-Aware Framework for Reproducible Biomarker Discovery and Precision Intervention Design in the Human Gut Microbiome. Briefings in Bioinformatics.

This repository is permanently archived at Zenodo with 
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19047082.svg)](https://doi.org/10.5281/zenodo.19047082)
