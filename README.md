# Reproduce_Thesis_InstitutCurie
This repository includes all code to reproduce the results from my Master's thesis named "Identification of genetic mechanisms controlling lineage commitment during human hematopoiesis".

### Input file
The four scATAC-seq files can be downloaded using SRA toolkit from https://www.ncbi.nlm.nih.gov/sra?term=SRP256229.  
Download SRR11539031.sra, SRR11539032.sra, SRR11539033.sra and SRR11539034.sra and put them in /data/sra/[sample]/[sample].sra

### Set up environment
1. Install conda environment
   `conda env create -f environment.yml`
2. Install Cell Ranger ATAC https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/installation
3. Install mgatk https://github.com/caleblareau/mgatk

### Run code
Run the bash scripts in the code folder in order 0 to 12.  
Script 5 (5_Annotation_example.R) should be executed for each sample indivually, assigning identity names based on results from the label transfer.
