# BIP-Erasmus.-Computational-Tools-in-Biopharma-Driving-Innovation-in-Drug-Discovery

Welcome to the course repository for the **Erasmus+ Blended Intensive Programme (BIP): Computational Tools in Biopharma – Driving Innovation in Drug Discovery**.

This repository brings together theoretical lectures, practical guides, interactive notebooks, molecular structures and supporting datasets. The course follows a computational drug discovery workflow, from the identification of potential therapeutic targets to molecular modelling, ligand–target docking and the analysis of molecular dynamics simulations.

## Learning objectives

By the end of the course, students should be able to:

- Explore genome-wide association study (GWAS) data and assess genetic evidence for potential therapeutic targets.
- Retrieve, visualize and interpret three-dimensional structures of biological macromolecules and small molecules.
- Prepare molecular structures and construct a membrane–protein model using computational tools.
- Set up and analyse molecular docking experiments, comparing predicted ligand poses with experimental structures.
- Analyse precomputed molecular dynamics (MD) trajectories to investigate structural stability, ligand–target interactions and energetic contributions.
- Interpret computational results critically, recognizing the limitations of each method in drug discovery.

## Course structure

The course is organized into four modules. Each module has its own README with learning objectives, software requirements, official download links and instructions for the practical sessions.

| Module | Topics and practical activities | Course materials |
| --- | --- | --- |
| **1. Omics Sciences for Target Identification** | GWAS data retrieval, Manhattan plots, Q–Q plots and genetic association analysis. | [Module 1 →](1.Omics_Sciences_for_Target_Identification/) |
| **2. Introduction to Molecular Structure** | Molecular visualization, small-molecule construction, protein–ligand structures and neuronal membrane modelling. | [Module 2 →](2.Introduction_to_Molecular_Structure/) |
| **3. Docking of Drug Candidates into Biological Targets** | Receptor and ligand preparation, search-space definition, molecular redocking and comparison of predicted and experimental poses. | [Module 3 →](3.Docking_of_Drug_Candidates_into_Biological_Targets/) |
| **4. MD Simulations for Drug–Target Interactions Analysis** | Trajectory analysis, RMSD, hydrogen bonds, cation–π interactions and MM-ISMSA energetic analysis. | [Module 4 →](4.MD_Simulations_for_Drug-Target_Interactions_Analysis/) |

## Software and online resources

Please review the README of each module before starting its practical session. Some tools require local installation, whereas others can be accessed directly through a web browser.

### Desktop applications and plugins

| Software | Purpose | Module | Official download / instructions |
| --- | --- | :---: | --- |
| PyMOL | Molecular visualization and structure preparation | 2, 3 | [Download PyMOL](https://pymol.org/installers/) |
| DockingPie | Molecular docking plugin for PyMOL | 3 | [Installation instructions](https://github.com/paiardin/DockingPie) |
| AutoDock Vina | Molecular docking engine | 3 | [Official website](https://vina.scripps.edu/) |

Install PyMOL before DockingPie, then follow the plugin's instructions to configure AutoDock Vina and any required dependencies. Check operating-system compatibility and licence requirements before downloading desktop software.

### Browser-based tools and databases

| Resource | Purpose | Module |
| --- | --- | :---: |
| [Google Colab](https://colab.research.google.com/) | Run Python notebooks without a local Python installation | 1, 4 |
| [GWAS Catalog](https://www.ebi.ac.uk/gwas/) | Access genome-wide association data | 1 |
| [RCSB Protein Data Bank (PDB)](https://www.rcsb.org/) | Access experimental macromolecular structures | 2, 3 |
| [CORINA Classic](https://demos.mn-am.com/corina_interactive.html) | Generate 3D molecular structures from SMILES | 2 |
| [CHARMM-GUI](https://www.charmm-gui.org/) | Build molecular systems and membrane models | 2 |
| [PLIP](https://plip-tool.biotec.tu-dresden.de/plip-web/plip/index) | Explore protein–ligand interactions (optional) | 2 |

The MD analysis notebook includes setup cells for CondaColab, AmberTools/CPPTRAJ and MMISMSA. No local molecular dynamics engine is required for the supplied trajectory-analysis exercise. Jupyter is an optional local alternative for the GWAS notebook.

## Interactive notebooks

The following notebooks can be opened directly in Google Colab:

| Practical session | Notebook | Run in Google Colab |
| --- | --- | --- |
| GWAS analysis workshop | [View notebook](1.Omics_Sciences_for_Target_Identification/WORSHOP1_GWAS_analysis-4alumn.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jyjlab210/BIP-Erasmus.-Computational-Tools-in-Biopharma-Driving-Innovation-in-Drug-Discovery/blob/main/1.Omics_Sciences_for_Target_Identification/WORSHOP1_GWAS_analysis-4alumn.ipynb) |
| Molecular dynamics analysis workshop | [View notebook](4.MD_Simulations_for_Drug-Target_Interactions_Analysis/MD-analysis.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jyjlab210/BIP-Erasmus.-Computational-Tools-in-Biopharma-Driving-Innovation-in-Drug-Discovery/blob/main/4.MD_Simulations_for_Drug-Target_Interactions_Analysis/MD-analysis.ipynb) |

To use a notebook, open it in Colab, connect to a runtime and run the setup and analysis cells in order. Save a personal copy to Google Drive if you wish to retain your changes. Download any results you want to keep before the runtime ends.

## Getting started

1. Open the relevant module using the links in the course structure table.
2. Read the module README and install any required desktop applications before the practical session.
3. Review the theoretical lecture materials and follow the corresponding practical guide or notebook.
4. Download the necessary input files, preserving their original names and folder structure. To download the repository as a whole, select **Code → Download ZIP** on GitHub; alternatively, download individual files as needed. Large files managed by Git LFS may need to be downloaded separately. The MD notebook retrieves its own simulation dataset automatically.
5. Work through the exercises, inspect the results and consider the biological meaning and limitations of your findings.

An internet connection is required for the web resources, Colab and external data downloads. No Git installation is required to access the course materials through the GitHub website.

### Note on molecular dynamics datasets

The [MD_results.tar.gz](4.MD_Simulations_for_Drug-Target_Interactions_Analysis/MD_results.tar.gz) archive available in Module 4 of this GitHub repository contains the molecular dynamics trajectories (`.nc` files) and the corresponding simulation movies generated from these trajectories. Students can download the archive to access the trajectories and view the simulation movies locally.

For convenience, the MD analysis notebook includes an automated download step that retrieves the simulation dataset directly from the course's Google Drive. Students therefore do not need to manually download or extract the GitHub archive to perform the analyses in Google Colab.

Access to the Google Drive dataset and the MMISMSA archive depends on the course file-sharing permissions. If the downloads fail or input files are missing, please contact the instructors before proceeding.

Note that previewing the notebook on GitHub does not execute the analyses. To run the practical exercises, open the notebook in Google Colab. For further instructions, see the [Module 4 README](4.MD_Simulations_for_Drug-Target_Interactions_Analysis/README.md).

## Scientific interpretation

The practical sessions illustrate complementary computational approaches to drug discovery. Genetic association is not proof of causation, a docking score is not a direct measurement of binding affinity, and MD-based structural and energetic estimates depend on the models and assumptions used. Computational predictions should be interpreted in context and, where appropriate, supported by experimental evidence.

## Support and references

If you encounter problems installing software, accessing data or running a practical exercise, consult the README and guides in the corresponding module or contact the course instructors.

Please acknowledge the original software developers, databases and scientific publications when using these tools and data in reports or presentations. References and documentation are provided in the module materials and linked resources.

## Contact information

For any questions regarding the course, practical sessions, software installation or access to the course materials, please contact the course instructors at Universidad Europea:

- [javier.acosta@universidadeuropea.es](mailto:javier.acosta@universidadeuropea.es)
- [jon.delarco@universidadeuropea.es](mailto:jon.delarco@universidadeuropea.es)
