# VisiumAnalysis

Scripts used for analysis of 10x Visium Spatial Transcriptome analysis. Includes SpaceRanger pipeline and bonus R script for plotting data

## SpaceRanger pipeline

Performed initially in WSL2 using Ubuntu 20.04.3.

Will only run in WSL2 on EXT4 formatted HDD partition.

Pipeline available from:

https://support.10xgenomics.com/spatial-gene-expression/software/downloads/latest

Input requirement:

- folder containing Illumina paired reads (R1 & R2) for each sample
- - .fastq files with naming conventions [SampleName]_S1_L00\[LaneNumber]\_[ReadNumber]_001.fastq.gz
- folder containing .tif files of scope images and .json alignment files from Loupe Browser manual alignment
- Slide Serial number and Slide area for each sample

## R for data plotting

### Version control

R analysis requires at least R version 4.0.0, Rtools4, and RStudio (at least 1.2.5042)

### Packages required

- ggplot2

- Matrix

- rjson

- cowplot

- RColorBrewer

- grid

- readbitmap

- Seurat

- dplyr

- hdf5r

- data.table


### Input requirements

Output files from SpaceRanger pipeline
