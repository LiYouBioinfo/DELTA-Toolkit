## DELTA-Toolkit
DNA Encoded Library Data Analysis toolkit for DEL data analysis \
By [You Li](https://www.linkedin.com/in/you-li-83a530aa/)


## About
**DELTA-Toolkit** (DEL_AnalysisToolkit_NAR.jar) is a compiled executable jar file that include modules for DNA-encoded library data QC, sequence analysis, feature identification and comparison, DNA binding motif prediction, etc. It is a proprietary software package developed by **HitGen lnc**. 

**HitGen** has established a drug discovery research platform for small molecules and nucleic acid drugs centered on the design, synthesis and screening of DNA encoded chemical libraries (DELs), fragment-based drug discovery (FBDD) and structure-based drug design (SBDD) technologies.

[Company Webpage](https://www.hitgen.com/en/)

## Publication 
Chen Q, Li Y, Lin C, Chen L, Luo H, Xia S, Liu C, Cheng X, Liu C, Li J, Dou D. Expanding the DNA-encoded library toolbox: identifying small molecules targeting RNA. Nucleic Acids Res. 2022 Mar 14:gkac173. doi: 10.1093/nar/gkac173. Epub ahead of print. PMID: 35288754. \
https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkac173/6548408

## Prerequisites
NEXT-RNAi prerequisites depend on the mode of running that is used. E.g. for designing or evaluating siRNAs solely based on their predicted efficiency, no prerequisites are required at all. Designing or evaluating long dsRNAs requires primer3 (for primer designs) in addition. The evaluation of the reagents' specificity further requires Bowtie (for alignments). All dependencies are listed and described below.

## Required software for a Linux installation
* perl
* nextrnai.pl (NEXT-RNAi perl script)
* LICENCE
* README
* bowtie (version 0.12.5)
* primer3 (version 1.1.1)
* blat (suite 34)
* blast (version 2.2.23)
* mdust
* ViennaRNA (version 1.8.4) 

## Get started
Read the installation instruction here: http://b110-wiki.dkfz.de/signaling/wiki/display/nextrnai/Installing+NEXT-RNAi

## Installation
Installation and testscripts are available for some OS, have a look at the directory: installation_scripts
