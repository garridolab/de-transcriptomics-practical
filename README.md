# Differential expression analysis of transcriptomic data

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/garridolab/de-transcriptomics-practical/blob/main/DE_analysis_PBMC_IFNb.ipynb)

A hands-on practical on differential expression (DE) analysis of RNA-seq counts with [PyDESeq2](https://github.com/owkin/PyDESeq2). It uses PBMCs from 8 donors, each with an untreated and an interferon-β-stimulated sample (pseudobulk counts derived from [Kang et al. 2018](https://doi.org/10.1038/nbt.4042)).

The notebook is self-contained:
- The first cell installs all dependencies with `pip`.
- The counts table is downloaded from Google Drive with `gdown`.

## Contents

| File | Description |
|---|---|
| `DE_analysis_PBMC_IFNb.ipynb` | The practical notebook |

## Topics covered

- Quality control and filtering
- Normalisation (size factors)
- Exploratory analysis: variance-stabilising transform (VST), PCA, sample distances
- Fitting the DESeq2 model and the dispersion plot
- Standard DE plots: p-value histogram, MA plot (with and without LFC shrinkage), volcano plot, heatmap of top genes, per-gene plots
- Paired vs unpaired experimental designs
- GO enrichment of the DE genes

## Running locally

```bash
jupyter lab DE_analysis_PBMC_IFNb.ipynb
```

Requires Python ≥ 3.10. The first cell installs everything else.
