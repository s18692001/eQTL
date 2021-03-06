## Introduction

The emerging research of bone biology through large-scale genomic techniques allows further investigation into prevalent bone diseases such as osteoporosis. Besides, several peer-reviewed publications have described significant explorations
of genome-wide association studies (GWAS) and expression quantitative trait loci (eQTL) analysis through cultured primary osteoblast cell lines, and discovered potential gene loci in regulatory networks for phenotypes like bone marrow density
(BMD). However, total bone biopsies, containing bone osteocytes and bone marrow composed of hematopoietic and stromal stem cells and their lineages such as endothelial and fibroblast cells, can demonstrate a composite cellular environment. Compared to bone research through cultured cell lines, whole bone biopsies are highly likely to obtain more intrinsic view of genetic regulation in bone biology and diseases. As a result, it is essential for bone disease researchers to exploit whole bone biopsies as model to understand regulatory networks through analyses such as GWAS and eQTL.

The efficiency of conducting GWAS analyses has resulted in accelerating breakthrough of the exploration of disease genetics in recent years. Moreover, many studies exploited BMD and osteoblast GWAS to understand bone diseases such as osteoporosis, and indicated potential functional genes. Although the GWAS method has already been favorable in determining novel candidate genes resulting in exploration of pathways involving in the pathophysiology, the genetic variants identified so far merely explain a little proportion of the heritability for complex traits. According to the lacking of genetic effect size and power to conquer the heterogeneity of genetic effects in meta-analyses, accurate association signals might not be unveiled depending only on a rigid genome-wide significance threshold. Furthermore, most GWAS analyses have not offered much evidence to identify novel genes that have not been investigated for a specific disease or trait before. As a result, it is necessary to combine supplementary information in the studies of GWAS. In the previous studies, researcher utilized gene expression profiles with signatures of cellular models to understand bone disease processes and metabolism, such as the study of parathyroid hormone (PTH) activated osteoclastogenesis and osteoblast development for osteoblastogenesis. The hormone, PTH, obliquely activated osteoclastogenesis through the receptor on osteoblast, then signaling to precursors on osteoclast to activate osteoclastogenesis. The defective osteoblast development resulted in osteoporosis in animal models and curtailed bone formation. In accordance with studies, one of the most notable candidate gene for osteoporosis, TNFRSF11B/OPG, demonstrated differential expression in cellular models is plausible to interfere in bone metabolism and associated with osteoporosis. GWAS-determined candidate genes, in contrast, did not show significant differential expression in cellular models. It could be uncertain which gene or SNP can be the cause, assuming that most reported significant SNPs in GWAS are in non-coding or in the intergenic regions. Besides, due to the fact that non-coding or intergenic SNPs don’t occur to influence protein peptide sequences, these SNPs may be placed in the transcription regulation elements of adjacent genes or in linkage disequilibrium (LD) with causal variants. As a result, in order to generate more trustworthy candidate causal SNPs, eQTL analyses in particular tissues is crucial by unification of phenotypic, transcriptomic and genetic variants dataset. This integrative analyses method may allow researchers to identify and obtain more reliable candidate genes. 

In order to identify the potential relationship between gene variants in whole bone and various phenotypes, in the current study, we conducted integrative analyses through whole bone eQTL and enrichment analyses with various GWAS. Furthermore, we also introduced experiments such as DNase I hypersensitive sites (DHSs) enrichment analysis to understand regulatory information of whole bone eQTL, GTeX eQTL, PBMC and osteoblast eQTLs enrichment analysis for further comprehension of whole bone eQTL. We first collected and processed whole bone eQTL and various GWAS datasets. After it, we utilized LD clustering algorithm and hypergeometric test to identify the significant characteristics between whole bone eQTL and various GWAS. Further analyses and overview of this study design are provided.

![Overview](https://github.com/s18692001/eQTL/blob/master/Overview.jpeg)


## Method and Scripts

# LD Clustering
Assign eQTL and GWAS SNPs in different Linkage Disequilibrium (LD) blocks by specific r square cut-off.

Script: baggingSNPsByLD.py

# Hypergeometric Test
Conduct Hypermetric Test for eQTL in different GWAS bins

![Hypergeometric Test](https://github.com/s18692001/eQTL/blob/master/hyper_test.png)

Script: hypergeometric_test_after_bagging.R, GWAS_enrichment_with_eQTL.R, GWAS_enrichment.py	



