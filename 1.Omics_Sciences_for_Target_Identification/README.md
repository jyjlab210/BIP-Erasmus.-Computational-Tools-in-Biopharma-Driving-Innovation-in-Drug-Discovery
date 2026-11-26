# 1. Omics Sciences for Target Identification

This module introduces omics-based target selection through a hands-on exploration of genome-wide association study (GWAS) data.

## Learning objectives

- Retrieve and clean genetic association data from the GWAS Catalog.
- Explore genomic positions, mapped genes and p-values using interactive Manhattan plots.
- Compare observed and expected p-values using Q–Q plots and interpret association evidence critically.

## Required software and online resources

| Tool | Purpose | Access / installation |
| --- | --- | --- |
| Google Colab (recommended) | Run the Python notebook in a browser | [Open Colab](https://colab.research.google.com/) |
| Jupyter (optional local alternative) | Run notebooks on your computer | [Installation instructions](https://jupyter.org/install) |
| GWAS Catalog | Association data and summary statistics | [GWAS Catalog](https://www.ebi.ac.uk/gwas/) · [API documentation](https://www.ebi.ac.uk/gwas/docs/programmatic-access/rest-api/) |

## Course materials

- [Omics Sciences — lecture slides](Omics_Sciences_BIP.pdf)
- [GWAS analysis workshop notebook](WORSHOP1_GWAS_analysis-4alumn.ipynb) — [Open in Google Colab](https://colab.research.google.com/github/jyjlab210/BIP-Erasmus.-Computational-Tools-in-Biopharma-Driving-Innovation-in-Drug-Discovery/blob/main/1.Omics_Sciences_for_Target_Identification/WORSHOP1_GWAS_analysis-4alumn.ipynb)

## Getting started

1. Open the notebook in Colab and connect to a Python runtime. Save a personal copy if you want to retain your work.
2. Run the setup cell and subsequent cells in order. The notebook retrieves data for trait `EFO_0004319` and study `GCST007460` from the GWAS Catalog.
3. If Python dependencies are missing, run the following in a notebook cell, restart the kernel and rerun the notebook:

   ```python
   %pip install pandas numpy requests plotly ipywidgets
   ```

4. Explore the interactive plots and gene filters, including the example gene `CHRNA4`.

An internet connection is needed to retrieve the data.
