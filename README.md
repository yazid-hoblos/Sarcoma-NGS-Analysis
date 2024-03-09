# Sarcoma-NGS-Analysis

## Overview

This repository attempt to understand the genetic and molecular (RNA level) changes that are responsible for the development and progression of Leiomyosarcoma (LMS), a type of rare cancer that grows in the smooth muscles. A detailed commentary on all the steps of analysis is provided in the RMarkdown document [LMS.Rmd](LMS.Rmd) and its compiled HTML equivalent [LMS.html](LMS.html).

## Alignment 

The _Rbowtie_ aligner of the _QuasR_ package was used to perform the alignment of the DNA reads in FASTQ format with the reference genome. 
Alternatively, the _Rhisat2_ aligner was used for the alignment of the RNA data, in parallel to the annotation of genes. 

## Quality Assessment 

The quality of the reads was assessed using _qQCReport_. The resulting metrics and plots on the quality of the [DNA](Alignment_quality.pdf) and [RNA](QCReport_RNAseq.pdf) reads are provided.

![image](https://github.com/yazid-hoblos/Sarcoma-NGS-Analysis/assets/125372209/fee4b7ae-4e2c-48cc-9d05-fde1bd2a507f)

## Visualization

Inspection of the final aligned reads derived from tumor and normal tissues revelead a potential duplication event around the gene MYOCD (myocardin), which plays a central role in the differentiation of the smooth muscle cell lineage.

![image](https://github.com/yazid-hoblos/Sarcoma-NGS-Analysis/assets/125372209/92a55d40-45c5-45e2-8a85-c4d269d8fd9f)

## RNAseq Analysis 

The gene expression around that region was also inspected. 

![image](https://github.com/yazid-hoblos/Sarcoma-NGS-Analysis/assets/125372209/32738d6c-954e-4a66-8af2-5464e70c1604)
