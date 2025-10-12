# 🧬 Epigenetic regulation of liver endothelial cells (LSECs) as a novel target to boost immunotherapy efficacy in hepatocellular cancer (HCC)

This project focuses on whether *EHMT2*, an epigenetic regulator, directly influences immune pathways and the endothelial-to-mesenchymal transition (*EndoMT*) in liver sinusoidal epithelial cells (LSECs) which aid in the development of *hepatocellular cancer* (HCC).

## Current Progress

```mermaid
gantt
    title Semester 1 Timeline
    dateFormat  DD-MM-YY
    axisFormat  %d/%m
    tickInterval 1week
    weekday monday

    section Video & Report
    Literature Review     :09-19-25,22-10-25
    1st Meeting w/ Deena & Obtain Data       :milestone, deena, 22-10-25, 1d
    Complete Video Pitch        :22-10-25, 08-12-25
    Video Pitch        :milestone, 15-01-26,1d
    Report 1st Draft      :after vis,13-01-26

    S1 End       :vert, v1, 13-12-25,1m

    section Analysis
    Real DAA + DEA      : real, after deena,3w
    GOA + Link: vis, after real, 2w
    Report Visualisations:   after vis, until v2

    S2 Start       :vert, v2, 12-01-26,1m

    section Publication Push

    DAA/DEA :practise, 13-10-25,until deena
    Propose Publication w/ Deena: proposal, after practise, 3w
    Scout Public DB for Meta-Analysis: meta, after proposal, until v1
```
## 🎯 Objectives

```mermaid
---
config:
  theme: dark
---
flowchart TB
    A["Raw ATACseq Data"] -- "QC, peak calling" --> B["Processed ATACseq Data"]
    B-- "DAA w/ DiffBind" -->C["Differentially Accessible Regions DARs"]
    D["Processed Bulk RNAseq Data"]-- "DEA w/ DESeq2" -->E["Differentially Expressed Genes DEGs"]

    X[ ]:::empty
    C --- X
    E --- X
    X --> F["DARs linked to DEGs"]

    Y[ ]:::empty
    F --- Y
    Y --> G["Role in EndoMT and immune pathways"]
    H["HCC Metadata Immune Markers"] --- Y

    classDef empty height: 0, width: 0
```

1) Analyse ATAC-seq data from LSECs with and without EHMT2 knockdown to identify alterations in chromatin accessibility regions influenced by EHMT2-mediated methylation.

2) Correlate ATAC-seq findings with bulk RNA-seq data from the same samples to determine how EHMT2’s downstream
effects influence gene transcription, particularly for EndoMT markers (e.g., αSMA, vimentin) and immune cell recruitment
pathways.

3) Identify key differentially accessible regions and associated genes that may explain EHMT2’s role in promoting immune
evasion in the HCC TME, supporting further experiments with human HCC samples and in vitro models (e.g., flow-based
adhesion assays investigating EHMT2 impact on immune cell recruitment).

## 📁 Files & Directories

```bash
bioinformatics-project/
├── docs/                    # essential and useful project docs
│   ├── tasks.docx
│   ├── minutes.docx
│   ├── report.pdf
│   ├── presentation.mov 
│   └── references.bib
├── notebooks/
├── data/
│   ├── raw/                  # symbolic links or small example subsets only
│   ├── processed/
│   └── metadata/             # sample info, config, manifests
├── scripts/
│   ├── preprocessing/ 
│   ├── analysis/             # main workflows
│   ├── visualization/
│   └── utils/                # helper functions
├── results/                  # publication-ready plots, tables, etc.
├── README.md
└── .gitignore                # list of files to not track
```


## 👥 Contributors

- Zhaoshuo Liu

- Yash Dhiman

- Simran Panda

- Miguel Alburo
