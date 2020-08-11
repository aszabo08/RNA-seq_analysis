This is a personal project in bioinformatics performing an RNA-seq analysis using Salmon for mapping the reads to the reference genome and DESeq2 for differential expression analysis.

**Background**: the experiment that generated the raw sequencing data I am using was conducted by Schmidt N, Domingues P, Golebiowski F, Patzina C et al. from University of Zurich [[1]](#1)
I accessed this publicly available data on Sequence Read Archive (SRA), under the SRA identifier "SRP212102" (<https://www.ncbi.nlm.nih.gov/sra?term=SRP212102>)
The aim of the experiment was to compare the differentially expressed genes in human lung epithelial cells expressing wild type TRIM28 or SUMOylation-deficient mutant TRIM28 (TRIM28 6KR) after influenza A infection.

Small Ubiquitin-like Modifier (SUMO) proteins participate in SUMOylation which is a post-translational modification process. They bound to target proteins and can alter their activity, stability and localization in the cell. In this experiment their involvement with transcriptional regulation is studied, in relation with Interferon regulatory factor 7 (IRF7).
IRF7 regulates the transcription of interferons, which are signalling proteins that result in virus induced defensive response from the immune system.
Tripartite motif–containing protein 28 (TRIM28) is a SUMO E3 ligase which is specific for IRF7 SUMOylation, resulting in repressed anti-viral response. [[2]](#2)

**Expectation**: by using wild type TRIM28 and SUMOylation-deficient TRIM28 6KR the difference after influenza infection can be compared. Cells with the former gene expected to have lower anti-viral response due to the impact of SUMOylation, while cells with the latter gene are predicted to have greater defensive response as their interferon transcription is not regulated negatively by IRF7.

**Experiment**: the experiment involved twelve samples out of which six contained cells expressing the wild type TRIM28 and six expressing TRIM28 6KR. In both groups three-three samples were mock infected and infected with influenza A virus at MOI=10 PFU/cell. RNA was extracted at 6 hours post infection.

**Analysis**: I describe my workflow in four separate Rmarkdown notebooks based on the following areas: pre-processing of the raw data, RNA-seq analysis of the samples expressing wild type TRIM28, RNA-seq analysis of the samples expressing TRIM28 6KR and the comparison of the last two results.

The rendered html files can be viewed on the links below:

* Bash scripts: [0_bash_scripts.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/0_bash_scripts.html)
* RNA-seq analysis of wild type TRIM28: [1_influenza_TRIM28_wt.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/1_influenza_TRIM28_wt.html)
* RNA-seq analysis of mutant TRIM28: [2_influenza_TRIM28_6KR.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/2_influenza_TRIM28_6KR.html)
* Comparison: [3_influenza_comparison.html](http://htmlpreview.github.io/?https://github.com/aszabo08/rna-seq_analysis/blob/master/3_influenza_comparison.html)


**References**

<a id="1">[1]</a >
Schmidt N, Domingues P, Golebiowski F, Patzina C et al.
An influenza virus-triggered SUMO switch orchestrates co-opted endogenous retroviruses to stimulate host antiviral immunity.
Proc Natl Acad Sci U S A 2019 Aug 27;116(35):17399-17408. PMID: 31391303

<a id="2">[2]</a >
Liang Q, Deng H, Li X, Wu X, Tang Q, Chang TH, Peng H, Rauscher FJ 3rd, Ozato K, Zhu F. Tripartite motif-containing protein 28 is a small ubiquitin-related modifier E3 ligase and negative regulator of IFN regulatory factor 7.
J Immunol. 2011 Nov 1;187(9):4754-63. doi: 10.4049/jimmunol.1101704. Epub 2011 Sep 21. PMID: 21940674; PMCID: PMC3197880.



