This is a personal project in bioinformatics performing RNA-seq analysis on A549 cells with or without influenza A virus infection.

Background: the experiment that generated the raw sequencing data I am using in this RNA-seq experiment was conducted by University of Zurich.
I accessed this publicly available data on Sequence Read Archive (SRA), under the SRA identifier "SRP212102" (<https://www.ncbi.nlm.nih.gov/sra?term=SRP212102>)

The aim of the experiment was to compare the differentially expressed genes in human lung epithelial cells expressing wild type TRIM28 or mutant TRIM28 (TRIM28 6KR) after influenza A infection.
Out of the total 12 samples 6 expressed the wild type gene and 6 expressed the mutant gene. In both groups 3-3 samples were mock infected and infected with influenza A virus at MOI=10 PFU/cell. RNA was extracted at 6 hours post infection.

I describe my workflow in four separate Rmarkdown notebooks based on the following areas: pre-processing of the raw data, RNA-seq analysis of the samples expressing wild type TRIM28, RNA-seq analysis of the samples expressing mutant TRIM28 and the comparison of these two datasets.

The rendered html files can be viewed on the links below:

* Bash scripts: [0_bash.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/0_bash.html)
* RNA-seq analysis of wild type TRIM28: [1_TRIM28_wt.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/1_TRIM28_wt.html)
* RNA-seq analysis of mutant TRIM28: [2_TRIM28_6KR.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/2_TRIM28_6KR.html)
* Comparison: [3_compare.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/3_compare.html)




