# VZV 2.0 annotation #

This repository contains files related to our recent re-annotation of VZV strain Dumas described here - [ mBio ](https://journals.asm.org/doi/10.1128/mBio.01568-20). 

All raw Illumina and Nanopore dRNA-Seq datasets associated with this study are available from the ENA under project accession [ PRJEB38829 ](https://www.ebi.ac.uk/ena/browser/view/PRJEB38829).

## Updates: ##

23.11.2021 - Fixed minor error with co-ordinates of VLT63 exons
24.08.2021 - Uploaded new version of GFF3 files and transcriptome file with minor fixes in genes 8 and 10, as well as in the VLT63 locus.


## Description of files: ##

### Annotation directory: ###
The major annotation files (GFF3 format) are found in the Annotation directory and comprise the following: 

- VZV-Dumas-Forward-2.0.gff3 - GFF3 file denoting all VZV RNAs annotated along the top strand of VZV strain Dumas
- VZV-Dumas-Reverse-2.0.gff3 - GFF3 file denoting all VZV RNAs annotated along the bottom strand of VZV strain Dumas 
- VZV_v2.0_complete.fasta - VZV 2.0 transcriptome file (multi-fasta) - contains all VZV transcripts present in the v2.0 annotation 

*Note: Users should ensure the header line in the genome fasta file matches the text used in column #1 of the GFF3 files prior to perform alignment and any downstream analyses*

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

- VZV-Dumas.fasta - original VZV strain Dumas genome sequence in FASTA format (Genbank accession NC_001348.1). This version is compatible with BED12 files in IGV.

*Note: these files were generated using nanopore dRNA-Seq datasets basecalled with Guppy v3.2.2*

*Note 2: BED12 filenames are constructured from VZV strain names (EMC1, pOka), infected cell type (ARPE-19 epithelial cells, hESC-derived neurons), infection period (12h, 24h, 96h), and treatment (cyclohexamide, phosphonoacetic acid) with the absence of CHX or PAA indicating no treatment was performed.*

