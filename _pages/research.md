---
layout: archive
title: ""
permalink: /research/
author_profile: true
---

Current Research
======
### Improving the computational efficiency of demographic inference from allele frequency spectra (AFS) with supervised machine learning

[Our research group](https://gutengroup.arizona.edu/) had previously developed the software package [dadi](https://dadi.readthedocs.io/en/latest/) for inferring demographic history using the diffusion approximation and composite likelihood. Inferring demography with dadi involves likelihood optimization, which can be very computationally expensive. In this project, we aim to improve the ease of use and lower the computational burden for dadi users with likelihood-free supervised machine learning. We trained a suit of multilayer perceptron regressors on dadi-simulated data and demonstrated that they can accurately and instantaneously predict various demographic parameters from input AFS. These trained regressors, therefore, offer significant improvement in computational efficiency without compromising accuracy. We also incorporate an accompanying method to quantify the uncertainty around each parameter prediction, a feature often lacking in most machine learning methods.

  * Conference presentations: 
     * [SMBE22 Talk](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/talk_smbe22.pdf)
     * [PEQG22 Poster](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/poster_peqg22.pdf)
     * [SMBE21 Poster](https://github.com/lntran26/lntran26.github.io/blob/a10c173c0186f65b92bf5168169bf7447f3acdfc/files/poster_smbe21.pdf)
  * Github Repo: [lntran26/dadi-ml](https://github.com/lntran26/dadi-ml)



### Developing a novel method for inferring the distribution of fitness effects (DFE) from single nucleotide polymorphism (SNP) alignments

The DFE of new mutations quantifies the input of mutations with certain selective effects (deleterious, neutral, advantageous) into natural populations and is central to many biological and evolutionary processes. Existing methods for DFE inference typically summarize the input genomic data into allele frequency spectra (AFS), which ignore patterns of linkage among SNPs in the data. Several groups have previously developed CNN-based methods to directly process SNP alignments that include linkage information, but none has applied it to DFE inference. In this project, we will build upon this SNP alignment based approach and further adapt it to the task of inferring the DFE. Our method will also incorporate more features in the data representation, such as the classification of synonymous versus non-synonymous variants. This novel approach to data representation is expected to be more informative and powerful than existing AFS-based DFE inference methods.

Past Research
======
### Viral and host determinants of human-cytomegalovirus-induced myelosuppression in hematopoietic progenitor cells

Human cytomegalovirus (HCMV) is a main cause of morbidity and mortality for patients undergoing transplantation due to its suppression of hematopoiesis down the myeloid lineage (myelosuppression). The molecular mechanisms by which HCMV dysregulates hematopoietic progenitor cell (HPC) causing myelosuppression is largely unknown. We have identified a viral protein, UL135, that is required for HCMV-mediated myelosuppression of infected HPCs. A mutant virus lacking UL135 fails to induce myelosuppression compared to wildtype virus. We have previously shown that UL135 downregulates the epidermal growth factor receptor (EGFR) expression and alters EGFR endocytic trafficking by interacting with host adaptor proteins CIN85 and Abi-1. EGFR is a major signaling hub with many downstream signaling pathways that regulate lineage-specific transcription factors and are intricately involved in many aspects of HPC maintenance and differentiation. Therefore, we hypothesize that UL135, through host interactor proteins CIN85 and Abi-1, downregulates EGFR downstream signaling and expression of myeloid-lineage-specific transcription factors, causing myelosuppression.

  * [Talk](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/LNT_2020.04.14_student_seminar.pdf)
  * [Poster](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/ul135_frontiers_symposium_2020.pdf)
