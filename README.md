# COI DADA2 boldigger cline pipeline

A DADA2 metabarcoding eDNA pipeline for COI marker using boldigger cline all working in R

## Required programs

1. R (https://www.r-project.org/)
2. DADA2 Bioconductor package (https://benjjneb.github.io/dada2/dada-installation.html)
3. Cutadapt (https://cutadapt.readthedocs.io/en/stable/installation.html)

## How to use the pipeline 

1. Download the R code on your local computer (or clone this directory)
2. Put all your demultiplexed sequences in a folder
3. Change file names to have the following pattern if not the case: Forward reads files end with "_R1_001.fastq", and Reverse reads files end with "_R2_001.fastq". Be careful not to include other "_" in your samples names.
4. Change the different paths in the R code to match your computer set-up (line 12 and line 46)
5. Change the primer for the one you are using in the R code (line 31 and line 33)
6. Change username and password line 233 and 234 for the BOLD plateform (register if not already)
7. You can start running the code ! 
8. Be carefull of looking at your quality profils before running line 102 to adapt your arguments, you can use the amplicon sequence tool I developped to look at your sequences and calculate the overlap to make sure you are not cutting to many base pairs 
9. Make sure you have a stable internet connection (and plenty of time) before running the boldigger cline code (line 244)
10. To create the bolean vector identifying blank samples line 327, replace "blank_identifier" line 329 by the characters identifying your blanks in your sample names
11. Be carefull along the code some objects dimensions will need updating

The different steps are very well explained in these tutorials : 
1. https://astrobiomike.github.io/amplicon/dada2_workflow_ex
2. https://benjjneb.github.io/dada2/tutorial.html

