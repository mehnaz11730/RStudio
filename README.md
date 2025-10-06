# Genome Analysis and Data Visualization with R
This repository contains R scripts and data files used for a comprehensive bioinformatics and data analysis assignment. The project focuses on two main areas:

# Comparative Genomics: 
Analyzing Coding DNA Sequences (CDS) of Escherichia coli (K-12 MG1655) and Campylobacter coli (GCA_003780985) to compare gene count, sequence length distribution, nucleotide/amino acid frequencies, and codon usage bias (RSCU).

# Biological Data Analysis: 
Processing and visualizing RNA-seq gene expression count data and statistical analysis of tree growth circumference data.

The analysis is structured across two primary R Markdown files, which contain all the code and interpretations.
# Project Structure
The repository includes the following key files and directories:

# MEHNAZ_MEEM_A4_part_1.Rmd
R Markdown file containing analysis for Gene Expression and Tree Growth Data.
# MEHNAZ_MEEM_A4_part_2.Rmd
R Markdown file containing analysis for Comparative Genomics (E. coli vs. C. coli).
# gene_expression.tsv
Input file for RNA-seq count data.
# growth_data.csv
Input file for tree circumference measurements.
# ecoli_cds.fa.gz
E. coli CDS fasta file (downloaded and unzipped by script).
# ccoli_cds.fa.gz
C. coli CDS fasta file (downloaded and unzipped by script).
# Dependencies
The R scripts rely on several packages, which must be installed in your R environment to run the analysis successfully.

# Required R Packages:
R.utils
Biostrings (Bioconductor)
kmer
seqinr
ggplot2
dplyr

# The entire analysis, including data download, processing, and visualization, is contained within the two R Markdown files (.Rmd).

# Execute the Code

To run the analysis and regenerate the output (including tables and plots):

Run in RStudio: Opened MEHNAZ_MEEM_A4_part_1.Rmd or MEHNAZ_MEEM_A4_part_2.Rmd, and use the "Knit" button. This will execute all code chunks and generate the final output documents (.html or .pdf versions).

The code automatically handles downloading the required large CDS fasta files from Ensembl Genomes/EBI.

# Key Findings

E. coli vs. C. coli Genome: E. coli exhibits a significantly larger gene set and total coding DNA length, reflecting its role as a generalist. C. coli is highly A/T-rich (low G+C content), which translates into a weaker codon bias favoring A- and T-ending codons.

Gene Expression: The vast majority of genes show low mean expression levels (as seen in the histogram plot), with the highest expressed genes belonging to the mitochondrial genome.

Growth Data: The analysis of tree circumference growth over a 10-year period showed that while the Northeast site had greater mean growth, the difference was not statistically significant based on the T-test (p \ge 0.05).
