# CancerCSP
Cancer dataset , early-stage, late-stage, clear cell renal cell carcinoma (ccRCC)
# Gene Expression-Based Biomarkers for Discriminating Early and Late Stage of Clear Cell Renal Cancer

## Overview
This study focuses on identifying gene expression-based biomarkers capable of distinguishing early-stage and late-stage clear cell renal cell carcinoma (ccRCC). The authors analyzed RNA-Seq gene expression data from 523 ccRCC patients obtained from The Cancer Genome Atlas (TCGA) database and developed multiple machine learning and threshold-based classification models.

The work aimed to reduce the large gene feature space into a compact biomarker panel that can accurately classify cancer stages while maintaining biological relevance. Different feature selection strategies, including threshold-based selection, Support Vector Machine (SVM)-based selection, and Weka-based correlation feature selection, were applied to identify highly discriminative genes.

The study identified several important biomarkers such as **NR3C2, ENAM, DNASE1L3, FRMPD2, PLEKHA9, MAP6D1, SMPD4,** and **C11orf73** that demonstrated significant differential expression between early and late stages of ccRCC.

Key findings include:

- Single-gene threshold models achieved up to **71.12% accuracy** using **NR3C2**.
- An 8-gene biomarker panel achieved **74.04% validation accuracy** with ROC of **0.80**.
- Weka-selected 64-gene models achieved **72.64% validation accuracy** with ROC of **0.81**.
- Gender-specific models showed improved predictive performance, suggesting differential genomic regulation between male and female ccRCC patients.
- A publicly accessible web server named **CancerCSP** was developed for stage prediction using RNA-Seq expression data.

The study demonstrates the importance of compact biomarker signatures and machine learning approaches in cancer stage prediction and prognosis.


webserver : https://webs.iiitd.edu.in/raghava/cancercsp/

zenodo : https://doi.org/10.5281/zenodo.20225603
---

Bhalla S, Chaudhary K, Kumar R, Sehgal M, Kaur H, Sharma S, Raghava GPS.  
**Gene expression-based biomarkers for discriminating early and late stage of clear cell renal cancer.**  
*Scientific Reports.* 2017;7:44997.  
DOI: https://doi.org/10.1038/srep44997

## Key Features

- RNA-Seq based biomarker discovery
- Threshold-based and machine learning classification models
- Support Vector Machine (SVM), Random Forest (RF), Naive Bayes, and J48 classifiers
- Weka-based feature selection
- Cancer hallmark GO-term enrichment analysis
- Gender-specific stage classification models
- Protein-protein interaction network analysis
- Web server implementation: **CancerCSP**

---

## Dataset Information

- Source: **TCGA KIRC (Kidney Renal Clear Cell Carcinoma)**
- Samples analyzed: **523 ccRCC patients**
- Expression format: **RSEM RNA-Seq values**
- Features analyzed: **~20,000 genes**
- Training dataset: **419 samples**
- Independent validation dataset: **104 samples**

---

## Important Biomarker Panels

### Combo-1 (8 Genes)
- NR3C2
- ENAM
- DNASE1L3
- FRMPD2
- PLEKHA9
- MAP6D1
- SMPD4
- C11orf73

### Weka-Based Feature Set
- 64 selected genes with highest discriminatory performance

### Cancer Hallmark Feature Set
- 38 genes associated with:
  - Apoptosis
  - DNA repair
  - Cell cycle
  - Cell adhesion
  - Immune response
  - Cell motility

---

### CancerCSP
The authors developed an online prediction server for classifying ccRCC stages using gene expression values.

Features include:
- Stage prediction module
- Gene expression analysis
- Threshold score analysis
- ROC-based biomarker evaluation

URL:
http://crdd.osdd.net/raghava/cancercsp/

---

## Conclusion

The study successfully identified compact and biologically meaningful biomarker signatures capable of differentiating early and late-stage clear cell renal cell carcinoma. The integration of machine learning, feature selection, and biological pathway analysis improved predictive accuracy while reducing feature dimensionality.

These biomarker panels may assist researchers and clinicians in understanding cancer progression and developing prognostic tools for ccRCC.

---
Author and contact 
Prof : Gajendra Pal Singh Raghava
Department of Computational Biology  
IIIT Delhi, India

