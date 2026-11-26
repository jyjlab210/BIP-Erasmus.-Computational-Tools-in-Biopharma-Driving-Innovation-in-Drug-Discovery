# 4. MD Simulations for Drug–Target Interactions Analysis

This module introduces molecular dynamics (MD) and analysis of precomputed trajectories for six nAChR receptor–ligand systems: Cytisinicline (C5E), Carbamoylcholine (CCE), Carbamoylcholine analogue (XRS), Varenicline (QMR), Nicotine (NCT), and Lobeline (L0B).

## Learning objectives

- Analyse structural stability (RMSD monitoring) and flexibility (RMSF monitoring).
- Analyse ligand–receptor interactions: hydrogen bonding and cation–π interactions.
- Compare MM-ISMSA energetic estimates and per-residue energy contributions.

## Required software and online resources

| Tool | Purpose | Access / installation |
| --- | --- | --- |
| Google Colab (recommended) | Execute the workshop notebook in a browser | [Open Colab](https://colab.research.google.com/) |
| CondaColab | Enable Conda/Mamba inside Colab | [Official repository](https://github.com/conda-incubator/condacolab) |
| AmberTools / CPPTRAJ | Structural trajectory analysis | [AmberTools package](https://anaconda.org/conda-forge/ambertools) · [CPPTRAJ](https://github.com/Amber-MD/cpptraj) |
| MMISMSA | Energetic analysis | Installed by the notebook from its course-provided Google Drive archive; [method reference](https://doi.org/10.1021/ct300497z) |

The notebook handles software installation in Colab; no local MD engine is required for this analysis exercise. The supplied code requests `ambertools==26.0`. Use the course-provided setup cells rather than installing a different version without checking with the instructors.

## Course materials

- [Theoretical Considerations of Molecular Dynamics Simulations](Theoretical_Considerations_of_Molecular_Dynamics_Simulations.pdf)
- [MD analysis workshop notebook](MD-analysis.ipynb) — [Open in Google Colab](https://colab.research.google.com/github/jyjlab210/BIP-Erasmus.-Computational-Tools-in-Biopharma-Driving-Innovation-in-Drug-Discovery/blob/main/4.MD_Simulations_for_Drug-Target_Interactions_Analysis/MD-analysis.ipynb)

## Getting started

1. Open the notebook in Colab, connect to a runtime and save a personal copy if needed.
2. Run the CondaColab installation cell. Allow the runtime to restart before continuing.
3. Run the AmberTools and MMISMSA installation cells. Only execute course-provided software from a trusted source.
4. Run the dataset-download cell, which uses `gdown` to retrieve `MD.zip` from Google Drive and extracts it into the runtime. Confirm the expected `MD/` directory is present.
5. Execute the structural and energetic analysis cells, then inspect the interactive plots and export results as instructed.

## Simulation data

The [`MD_results.tar.gz`](MD_results.tar.gz) archive available in this GitHub repository contains the molecular dynamics trajectories (`.nc` files) and the corresponding simulation movies generated from these trajectories.

For convenience, the Google Colab notebook includes an automated download step that retrieves the simulation dataset directly from Google Drive, so students do not need to manually download or extract the archive from GitHub to perform the analyses.

Access to the Google Drive dataset and the MMISMSA archive depends on the course file-sharing permissions. If the downloads fail or input files are missing, please contact the instructors before proceeding.

Note that previewing the notebook on GitHub does not execute the analyses. To run the practical exercises, open the notebook in Google Colab.

## Reference

Klett et al. (2012), *MM-ISMSA: An Ultrafast and Accurate Scoring Function for Protein-Protein Docking*, [DOI: 10.1021/ct300497z](https://doi.org/10.1021/ct300497z).
