---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

Main Projects
======
### donni: Inferring population history with uncertainty quantification using Mean-Variance Estimation network

Inferring past demographic history of natural populations from genomic data is of central concern in many studies across research fields. [Our research group](https://gutengroup.arizona.edu/) had previously developed the widely used software package [dadi](https://dadi.readthedocs.io/en/latest/) for inferring demographic history using allele frequency spectrum (AFS) data and maximum likelihood optimization. However, dadi's likelihood optimization procedure is computationally expensive and inefficient. Here, I led a team effort in the development of donni (demographic history optimization via neural network inference), a new inference method based on dadi that is more efficient while maintaining comparable inference accuracy to dadi. donni consists of trained regressor networks for a large collection of commonly used demographic history models along with options for advanced users to train their own networks for custom models. donni also incorporates an accompanying method to quantify the uncertainty around each inferred value, a feature often lacking in most machine learning methods.

  * Conference presentations: 
     * [SMBE22 Talk](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/talk_smbe22.pdf)
     * [PEQG22 Poster](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/poster_peqg22.pdf)
     * [ProbGen23 Poster](https://github.com/lntran26/lntran26.github.io/blob/cad07df03dfb99264b8a048a2f25c0503b0cda5a/files/PROBGEN_23_Tran.pdf)
  * Github Repo: [lntran26/donni](https://github.com/lntran26/donni)
  * Publication: Tran, L. N., Sun, C. K., Struck, T. J., Sajan, M., & Gutenkunst, R. N. (2023). Computationally efficient demographic history inference from allele frequencies with supervised machine learning. bioRxiv. [link](https://www.biorxiv.org/content/10.1101/2023.05.24.542158v2)

### DFEnn: Inferring the distribution of fitness effects (DFE) of deleterious mutations using convolutional neural network and a novel genomic data representation with functional annotations

The distribution of fitness effects (DFE) of new mutations quantifies the input of mutations with certain selective effects (deleterious, neutral, advantageous) into natural populations and is fundamental to evolution by natural selection. The DFE is particularly important for understanding quantitative traits, such as the genetic architecture of complex diseases. All previous studies that estimated the DFE from genetic variation data used summary statistics describing some aspects of the data, such as the allele frequency spectrum and/or linkage disequilibrium statistics. While powerful, these existing approaches either neglect substantial information from the data not included in the chosen summary statistics or demand careful curation of the appropriate set of summary statistics. Here I have been developing the first deep learning approach for DFE inference using convolutional neural network (CNN) and a novel representation of genetic variation data. Single nucleotide polymorphism (SNP) alignment is represented by a three-dimensional tensor in which each layer corresponds to a functional class, such as synonymous and nonsynonymous coding variants. With this representation, our approach allows direct processing of genetic variation data in which the CNN implicitly learns the most informative features in the data, bypassing summary statistics selection and assumption.

  * Conference presentations: 
     * [ASHG23 Talk](https://github.com/lntran26/lntran26.github.io/blob/1ce0360190b2b543149041065fe9085eaf6578b7/files/LNT_ASHG_final.pdf)
  * Github Repo: [lntran26/dfenn](https://github.com/lntran26/dfenn)

### ConfuseNN: Interpreting convolutional neural networks inferences in population genomics by data shuffling

Convolutional neural network (CNN) is an increasingly popular supervised machine learning approach that has been applied to many inference tasks in population genetics. Under this framework, population genomic variation data are typically represented as 2D images with sampled haplotypes as rows and segregating sites as columns. While many published studies reported promising performance of CNNs on various inference tasks, understanding which features in the data were picked up by the CNNs and meaningfully contributed to the reported performance remains challenging. In this work, I implement a novel approach to interpreting CNN performance motivated by population genetic theory on genomic data. The final product is a suite of scramble tests where each test deliberately disrupts a feature in the genomic image data (e.g. allele frequency, linkage disequilibrium, etc.) to assess how each feature affects the CNN performance. I apply these tests to three networks designed to infer demographic history and natural selection, identifying the fundamental population genomic features that drive inference for each network.

  * Conference presentations: 
     * [TAGC24 Poster](https://github.com/lntran26/lntran26.github.io/blob/4e461eaf627614b75ec47d9a8f72fd5491880fb9/files/TAGC_24_Tran_final.pdf)
  * Github Repo: [lntran26/ConfuseNN](https://github.com/lntran26/ConfuseNN)

Side Projects
======
### Validation of an approach to model the allele frequency spectra for low-coverage sequencing data
[Our research group](https://gutengroup.arizona.edu/)'s software package [dadi](https://dadi.readthedocs.io/en/latest/) infers demographic history and the distribution of fitness effects (DFE) using the allele frequency spectra (AFS) summarized from genetic data as an input. Low-coverage genome sequencing is a popular and cost-effective method used in many studies but can introduce a significant bias into the AFS during downstream analysis. To address this problem, our lab developed a probabilistic model to account for the distortions induced by low-coverage sequencing and incorporated it into dadi. I contributed to the validation of this approach by applying it to NGS data from the 1000 Genomes Project and comparing its performance to an existing approach, ANGSD.

  * Github Repo: [lntran26/low-coverage-sfs](https://github.com/lntran26/low-coverage-sfs)

### stdpopsim: a community-maintained standard library of population genetic models
[The PopSim Consortium](https://github.com/popsim-consortium) is an open-source collaborative project with the goal of providing standardized simulation models and simulation engine backends for the population genetic research community. I'm contributing to the development of a snakemake analysis pipeline showcasing the use of stdpopsim in simulating and inferering population history and natural selection.
  
  * Github Repo: [lntran26/analysis2](https://github.com/lntran26/analysis2)

Past Project
======
### Viral and host determinants of human-cytomegalovirus-induced myelosuppression in hematopoietic progenitor cells

Human cytomegalovirus (HCMV) is a main cause of morbidity and mortality for patients undergoing transplantation due to its suppression of hematopoiesis down the myeloid lineage (myelosuppression). The molecular mechanisms by which HCMV dysregulates hematopoietic progenitor cell (HPC) causing myelosuppression is largely unknown. We have identified a viral protein, UL135, that is required for HCMV-mediated myelosuppression of infected HPCs. A mutant virus lacking UL135 fails to induce myelosuppression compared to the wild-type virus. We have previously shown that UL135 downregulates the epidermal growth factor receptor (EGFR) expression and alters EGFR endocytic trafficking by interacting with host adaptor proteins CIN85 and Abi-1. EGFR is a major signaling hub with many downstream signaling pathways that regulate lineage-specific transcription factors and are intricately involved in many aspects of HPC maintenance and differentiation. Therefore, we hypothesize that UL135, through host interactor proteins CIN85 and Abi-1, downregulates EGFR downstream signaling and expression of myeloid-lineage-specific transcription factors, causing myelosuppression.

  * [Talk](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/LNT_2020.04.14_student_seminar.pdf)
  * [Poster](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/ul135_frontiers_symposium_2020.pdf)
  * Publication: Mlera, L., Moy, M., Maness, K., Tran, L. N., & Goodrum, F. D. (2020). The role of the human cytomegalovirus UL133-UL138 gene locus in latency and reactivation. Viruses, 12(7), 714. [link](https://doi.org/10.3390/v12070714)
