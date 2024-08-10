## Overview

VariantSeq-Pipeline is a comprehensive bioinformatics pipeline for processing DNA sequencing data and identifying genomic variants. This pipeline automates the steps from downloading raw sequencing data to generating a VCF (Variant Call Format) file, providing a streamlined and efficient workflow for variant calling.

# Requirements

1. Conda (Anaconda or Miniconda)
2. Internet connection for downloading data and tools

# Pipeline Steps:

1. Sets up the conda environment and installs required tools.
2. Downloads raw sequencing reads (FASTQ files) and the reference genome.
3. Fetches the reference genome using Biopython.
4. Trims the sequencing reads to remove low-quality bases.
5. Aligns the trimmed reads to the reference genome.
6. Converts the alignment from SAM to BAM, sorts the BAM file, and generates mapping statistics.
7. Calls variants and outputs them in VCF format.

# Output Files:

1. output.sorted.bam: Sorted BAM file of the aligned reads.
2. variants.raw.vcf: VCF file containing the called variants.
3. mappingstats.txt: Alignment statistics.

# File Structure
1. dna_seq_pipeline.sh: The main script for executing the pipeline.
2. README.md: This documentation file.
