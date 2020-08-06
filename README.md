# VZV 2.0 annotation #

This repository contains files related to our recent re-annotation of VZV strain Dumas described here - [ bioRxiv ](https://www.biorxiv.org/content/10.1101/2020.05.25.110965v1). 

All raw Illumina and Nanopore dRNA-Seq datasets associated with this study are available from the ENA under project accession [ PRJEB38829 ](https://www.ebi.ac.uk/ena/browser/view/PRJEB38829).

## Description of files: ##

### Annotation directory: ###
The major annotation files (GFF3 format) are found in the Annotation directory and comprise the following: 

- VZV-Dumas-Forward-2.0.gff3 - GFF3 file denoting all VZV RNAs annotated along the top strand of VZV strain Dumas
- VZV-Dumas-Reverse-2.0.gff3 - GFF3 file denoting all VZV RNAs annotated along the bottom strand of VZV strain Dumas 
- VZV-Dumas.fasta - original VZV strain Dumas genome sequence in FASTA format (Genbank accession NC_001348.1) 

*Note:Users should ensure the header line in the genome fasta file matches the text used in column #1 of the GFF3 files prior to perform alignment and any downstream analyses*

### BED12 directory: ###
BED12 format files containing FLAIR-corrected read alignments are found in the BED12 folder and comprise the following:

- EMC1_ARPE19_12h_CHX_for_corr_all_corrected.bed
- EMC1_ARPE19_12h_CHX_rev_corr_all_corrected.bed
- EMC1_ARPE19_24h_PAA_for_corr_all_corrected.bed
- EMC1_ARPE19_24h_PAA_rev_corr_all_corrected.bed
- EMC1_ARPE19_24h_for_corr_all_corrected.bed
- EMC1_ARPE19_24h_rev_corr_all_corrected.bed
- EMC1_ARPE19_96h_for_corr_all_corrected.bed
- EMC1_ARPE19_96h_rev_corr_all_corrected.bed

- pOka_NEU_96h_for_corr_all_corrected.bed
- pOka_NEU_96h_rev_corr_all_corrected.bed

- pOka_ARPE19_96h_biorep1_for_corr_all_corrected.bed
- pOka_ARPE19_96h_biorep1_rev_corr_all_corrected.bed
- pOka_ARPE19_96h_biorep2_for_corr_all_corrected.bed
- pOka_ARPE19_96h_biorep2_rev_corr_all_corrected.bed

*Note: these files were generated using nanopore dRNA-Seq datasets basecalled with Guppy v3.2.2*

