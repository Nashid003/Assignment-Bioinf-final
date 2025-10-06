# Assignment-Bioinf-final
final assignment # Bioinformatics Assignment

Bioinformatics Analysis: Gene Expression, Tree Growth, and Sequence Diversity
This repository contains an R workflow for analyzing gene expression data, tree growth measurements, and biological sequence diversity. The analyses are divided into two parts: Part 1 focuses on RNA-seq gene expression data and tree circumference measurements, while Part 2 examines coding sequence diversity in Escherichia coli and Clostridium baratii.
Features
Part 1: Gene Expression and Tree Growth Analysis

Data Import and Wrangling: Import and process RNA-seq count data (gene_expression.tsv) and tree circumference measurements (growth_data.csv).
Statistical Analysis: Compute mean gene expression, identify highly and lowly expressed genes, and calculate tree growth statistics (mean, standard deviation, and 10-year growth differences).
Visualization: Generate histograms for mean gene expression and boxplots for tree circumference distributions by site.
Statistical Testing: Perform a Welch Two Sample t-test to compare 10-year tree growth between sites.

Part 2: Biological Sequence Diversity

Sequence Analysis: Compare coding DNA sequences (CDS) from E. coli and C. baratii using FASTA files from Ensembl Genomes.
Sequence Metrics: Calculate the number of coding sequences, total coding DNA length, and mean/median CDS lengths.
Frequency Analysis: Compute nucleotide and amino acid frequencies, and visualize with barplots.
Codon Usage: Analyze codon usage bias using Relative Synonymous Codon Usage (RSCU) and visualize with barplots.
K-mer Analysis: Identify over- and under-represented protein k-mers (length 3–5) in C. baratii and compare with E. coli, supported by barplots.

Repository Contents

part1_analysis.R: Script for gene expression and tree growth analysis.
Outputs: Tables of gene expression, top 10 highly expressed genes, count of low-expression genes, mean/SD of tree circumferences, and 10-year growth t-test results.
Visualizations: Histogram of mean gene expression, boxplots of tree circumferences (2005 and 2020).


part2_sequence_analysis.R: Script for biological sequence diversity analysis.
Outputs: Tables of CDS counts and total coding DNA, mean/median CDS lengths, nucleotide/amino acid frequencies, codon usage (RSCU), and top/bottom k-mers.
Visualizations: Boxplots of CDS lengths, barplots of nucleotide/amino acid frequencies, codon usage, and k-mer frequencies.


data/: Directory containing input files (if hosted locally):
gene_expression.tsv: RNA-seq count data.
growth_data.csv: Tree circumference measurements.
ecoli_cds.fa: E. coli coding sequences.
cbar_cds.fa: C. baratii coding sequences.


figures/: Directory for output plots (e.g., histograms, boxplots, barplots).
functions.R: Custom utility functions for data processing and visualization.

Data Sources

Gene Expression and Tree Growth Data: Sourced from https://github.com/ghazkha/Assessment4.
Coding Sequence Data: FASTA files from Ensembl Genomes (release-62):
E. coli: Escherichia_coli_str_k_12_substr_mg1655_gca_000005845.
C. baratii: Clostridium_baratii_gca_001405755.



Authors
Developed by Nashid.
