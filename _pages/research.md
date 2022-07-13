---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

Current Research
======
### Improving the computational efficiency of demographic inference from allele frequency spectra with supervised machine learning

Our group had previously developed the software package [dadi](https://dadi.readthedocs.io/en/latest/) for inferring demography that supports a wide range of demographic models but expensive likelihood computation limits scalability. We can bypass this bottleneck and improve efficiency by employing likelihood-free approaches such as neural network (NN) algorithms. I'm developing a NN-based method for inferring all demographic models currently supported by dadi, and generate a suite of estimators that can accurately and instantaneously infer various demographic parameters. These NN-based estimators will offer significant improvement in computational efficiency without compromising inference accuracy. Additionally, our trained estimators will incorporate an accompanying method to quantify the uncertainty around each estimated parameter, a feature currently lacking in most NN-based inference methods.

  * Conference presentations: 
     * [SMBE22 Talk](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/talk_smbe22.pdf)
     * [PEQG22 Poster](https://github.com/lntran26/lntran26.github.io/blob/ce5c17d6de820050066c1c44ac23f17a2773a052/files/poster_peqg22.pdf)
     * [SMBE21 Poster](https://github.com/lntran26/lntran26.github.io/blob/a10c173c0186f65b92bf5168169bf7447f3acdfc/files/poster_smbe21.pdf)
  * Github Repo: [lntran26/dadi-ml](https://github.com/lntran26/dadi-ml)



### Developing a novel image-based CNN method for inferring the distribution of fitness effects (DFE) from single nucleotide polymorphism (SNP) alignments

The DFE of new mutations quantifies the input of mutations with certain selective effects (deleterious, neutral, advantageous) into natural populations and is central to the mechanisms of many biological processes. All existing methods infer the DFE from summary statistics derived from SNP data, leading to unavoidable information loss. Several groups have developed NN-based methods to directly process SNP alignments, but none has applied it to DFE inference. I plan to build upon this SNP alignment based approach and further adapt it to the task of inferring the DFE. Our approach will incorporate functional features such as classification of synonymous and non-synonymous variants in the data representation. This novel approach to data representation is expected to be more informative and powerful than existing frequency-spectrum-based DFE inference methods.

Past Research
======
### Viral and host determinants of human-cytomegalovirus-induced myelosuppression in hematopoietic progenitor cells

Human cytomegalovirus (HCMV) is a main cause of morbidity and mortality for patients undergoing transplantation due to its suppression of hematopoiesis down the myeloid lineage (myelosuppression). The molecular mechanisms by which HCMV dysregulates hematopoietic progenitor cell (HPC) causing myelosuppression is largely unknown. We have identified a viral protein, UL135, that is required for HCMV-mediated myelosuppression of infected HPCs. A mutant virus lacking UL135 fails to induce myelosuppression compared to wildtype virus. We have previously shown that UL135 downregulates the epidermal growth factor receptor (EGFR) expression and alters EGFR endocytic trafficking by interacting with host adaptor proteins CIN85 and Abi-1. EGFR is a major signaling hub with many downstream signaling pathways that regulate lineage-specific transcription factors and are intricately involved in many aspects of HPC maintenance and differentiation. Therefore, we hypothesize that UL135, through host interactor proteins CIN85 and Abi-1, downregulates EGFR downstream signaling and expression of myeloid-lineage-specific transcription factors, causing myelosuppression.

  * [Talk](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/LNT_2020.04.14_student_seminar.pdf)
  * [Poster](https://github.com/lntran26/lntran26.github.io/blob/b49bec4f3bc73d6a082b50f53ada3a50a9b112f2/files/ul135_frontiers_symposium_2020.pdf)
