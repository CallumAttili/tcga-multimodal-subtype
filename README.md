Molecular Data Type Subsets Outperform Full Multi-Omic Models for Cancer Subtype Classification
Callum Attili | UC Santa Cruz, Biomolecular Engineering | Capstone Project


Overview
This repository contains the code and data manifests for a multi-modal deep learning study of cancer subtype classification using TCGA data. The core finding is that optimal modality subsets are cancer-specific and consistently outperform full six-modality models for within-cancer subtype classification. Systematic ablation across all 63 modality combinations across five cancer cohorts reveals that the identity of the best subset tracks the underlying biology of each cancer's subtypes.


Data
All molecular and clinical data are publicly available through the NCI Genomic Data Commons (GDC) at https://portal.gdc.cancer.gov under the TCGA program (dbGaP accession phs000178). No controlled-access data were used.

Six modalities were downloaded via the GDC REST API:

Modality
data_category
data_type
workflow_type
RNA-seq
Transcriptome Profiling
Gene Expression Quantification
STAR - Counts
Methylation
DNA Methylation
Methylation Beta Value
SeSAMe Methylation Beta Estimation
CNV
Copy Number Variation
Gene Level Copy Number
AscatNGS
miRNA
Transcriptome Profiling
miRNA Expression Quantification
BCGSC miRNA Profiling
Mutations
Simple Nucleotide Variation
Masked Somatic Mutation
MuTect2
Clinical
Clinical
Clinical Supplement
n/a


Molecular subtype labels were obtained from the TCGA PanCanAtlas: https://www.cell.com/pb-assets/consortium/pancanceratlas/pancani3/index.html


Requirements
Python 3.10
PyTorch 2.0 (CUDA 11.8)
NumPy 1.24
pandas 2.0
scikit-learn 1.3
umap-learn 0.5
matplotlib 3.7

Install with:

pip install torch numpy pandas scikit-learn umap-learn matplotlib



Citation
If you use this code or data, please cite:

Attili C. Molecular data type subsets outperform full multi-omic models for cancer subtype classification. UC Santa Cruz BME 129C Capstone. 2026.


Contact
Callum Attili | callumattili@yahoo.com
