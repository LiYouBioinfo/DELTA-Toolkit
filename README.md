# DELTA-Toolkit
DNA Encoded Library Data Analysis toolkit for DEL data analysis (Author: [You Li](https://www.linkedin.com/in/you-li-83a530aa/))

### About DELTA-Toolkit
**DELTA-Toolkit** (DEL_AnalysisToolkit_NAR.jar) is a compiled executable jar file that include modules for DNA-encoded library data QC, sequence analysis, feature identification and comparison, DNA binding motif prediction, etc. It is a proprietary software package currently maintained by **HitGen Inc**. 

### About HitGen Inc.
**HitGen Inc** ([Home Page](https://www.hitgen.com/en/)) is a biotech company headquartered in Chengdu, China, with subsidiaries in Cambridge, UK and Houston, USA. HitGen became a publicly listed company in Shanghai Stock Exchange in April 2020 (ticker code 688222.SH) and  has established a drug discovery research platform for small molecules and nucleic acid drug centered on the design, synthesis and screening of DNA encoded chemical libraries (DELs), fragment-based drug discovery (FBDD) and structure-based drug design (SBDD) technologies. HitGen's DELs currently contains more than 1 trillion novel, diverse, drug-like small molecules and macrocyclic compounds. These compounds are members of DELs synthesized from many thousands of distinct chemical scaffolds, designed with tractable chemistry, and have yielded proven results for the discovery of small molecule leads against precedented and unprecedented classes of biological targets. 

### Publication 
Chen Q, Li Y, Lin C, Chen L, Luo H, Xia S, Liu C, Cheng X, Liu C, Li J, Dou D. Expanding the DNA-encoded library toolbox: identifying small molecules targeting RNA. Nucleic Acids Res. 2022 Mar 14:gkac173. doi: 10.1093/nar/gkac173. Epub ahead of print. PMID: 35288754. \
https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkac173/6548408

# Prerequisites
All dependencies for DELTA toolkit are listed below.

**List of dependencies**
* [cutadapt](https://cutadapt.readthedocs.io/en/stable/)
* [java jdk (or jre) v1.8 or above](https://www.oracle.com/java/technologies/downloads/)
* [R (with ggplot2, gridExtra and reshape2)](https://www.r-project.org/)
* [samtools](http://www.htslib.org/)
* [pigz](https://zlib.net/pigz/)

**Optional Softwares**
* [DataWarrior](https://openmolecules.org/datawarrior/) \
DataWarrior is not required for running the DELTA toolkit. However, it is needed for downstream file visualization (DELTA toolkit creates output for each DEL in *.dwar format).

### Install cutadapt via pip
```
pip install --user --upgrade cutadapt
```

### Install java JDK1.8 
Use the following command with caution. You may want to customize the installation.
```
yum install java-1.8.0-openjdk* -y
```

### Install R version 3.4.1 or higher
```
yum install epel-release
yum install R
```

### in R, install the following packages
```
install.packages("ggplot2");
install.packages("gridExtra");
install.packages("reshape2");
```

### Install samtools
```
wget https://github.com/samtools/samtools/releases/download/1.9/samtools-1.9.tar.bz2
tar jxf samtools-1.9.tar.bz2
cd samtools-1.9/
./configure --prefix=/where/to/install
make
make install
export PATH=/where/to/install/bin:$PATH
```

make sure when you type "samtools", the description of the tool is shown in the terminal.

### Request a copy of the DELTA toolkit
Please send an email to **you.li at hitgen.com** with the following information to request a copy of the toolkit (**DEL_AnalysisToolkit_NAR.jar**). Failed to include the correct information may lead to delayed response.

An example email should at least include the following information...

Email subject: 
> **[DELTA] Requesting a copy of DELTA toolkit.**

Email Body:
> Name: XXXX \
> Company/Institute：XXXXXX 

Or click the link below for the email template: 
<a href="mailto:you.li@hitgen.com?subject=[DELTA]%20Requesting%20a%20copy%20of%20DELTA%20toolkit.&body=Name:%0d%0aCompany/Institute">Requesting for a copy of DELTA toolkit</a>

### Deploy DEL_AnalysisToolkit_NAR.jar
**DEL_AnalysisToolkit_NAR.jar** is a compiled executable jar file that requires no installation. Simply put the jar file in your local directory and invoke the toolkit by using the following command: 

```
java -jar /path/to/your/DEL_AnalysisToolkit_NAR.jar
```

Please note that although executable jar file should be platform-independent. However, the software package was only extensively tested in the Unix-like OS. Therefore, the performance of this package is not guaranteed on Mac OS or Windows OS.

# Get started
A detailed description about the data analysis workflow and algorithms behind the toolkit, can be found in the supplementary data ([link](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkac173/6548408#340466457)) section of the published manuscript (doi: 10.1093/nar/gkac173).

Read the user manual here: https://github.com/LiYouBioinfo/DELTA-Toolkit/wiki

# FAQs (or report a bug)
Please check the [issue](https://github.com/LiYouBioinfo/DELTA-Toolkit/issues) page before posting.
