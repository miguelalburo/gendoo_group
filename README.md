# 🧬 Epigenetic regulation of liver endothelial cells (LSECs) as a novel target to boost immunotherapy efficacy in hepatocellular cancer (HCC)

## 🔍 Background
The overarching research question is: “How can epigenetic regulation of the tumour endothelium be targeted to reprogramme the immune microenvironment of liver cancer?” This question addresses the challenges in treating hepatocellular carcinoma (HCC), a leading cause of cancer-related mortality globally, with rising incidence in the UK. The tumour microenvironment (TME) promotes immune evasion, limiting the efficacy of immunotherapy in HCC. Liver sinusoidal endothelial cells (LSECs) undergo endothelial-to-mesenchymal transition (EndoMT), fostering a pro-angiogenic state that contributes to immunosuppression. Preliminary bulk RNA-seq data indicates that the epigenetic regulator EHMT2 is significantly upregulated in LSECs in HCC, correlating with increased infiltration of pro-cancer immune cells and poorer patient outcomes in publicly available data. We hypothesize that EHMT2 drives EndoMT and immune cell recruitment through histone and non-histone methylation, suggesting that targeting EHMT2 could reverse these epigenetic changes to develop novel therapeutic strategies.

## 🎯 Objectives
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
