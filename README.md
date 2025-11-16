# ligand-pocket-filtering-pipeline
A Python-based ligand–pocket filtering pipeline developed for my MSc thesis at the Royal College of Surgeons in Ireland (RCSI).
The project integrates Fpocket, RDKit, Py3Dmol, and machine learning to analyse protein binding pockets and prioritise compatible ligands for early-stage drug discovery.
Designed to be fully interactive, beginner-friendly, and reproducible inside a Jupyter environment.

This pipeline helps researchers analyse protein binding pockets and evaluate ligand compatibility at scale.
It enables:
Pocket Detection

Automated detection of binding pockets using Fpocket

Extraction of descriptors (volume, polarity, hydrophobicity)

Calculation of pocket centroids for downstream docking and filtering

2. Ligand & Residue Analysis

Ligand centroid extraction

Distance calculations between ligand and pockets

Identification of surrounding amino acid residues

Optional ligand inclusion/exclusion modes

Visualisation of protein, pocket, and ligand using Py3Dmol

3. Compound Filtering

Works with ZINC22 and other large chemical libraries

RDKit-based descriptors:

LogP

Heavy atom count

ElectroShape-style volume estimation

Matching ligand properties to pocket features

Supports large-scale filtering (10,000+ molecules)

4. Machine Learning Prioritisation (Optional)

Random Forest ligand ranking

Feature importance plots

PCA and clustering

Radar plots for chemical profiling

5. Docking Integration (Optional)

AutoDock Vina support

Automatic grid box generation from pocket centroids

Ligand and receptor preparation (PDB → PDBQT)

Docked pose visualisation

🧠 Technologies Used

Python: RDKit, NumPy, Pandas, Scikit-learn, Py3Dmol

Structural Bioinformatics: Fpocket, PDB parsing

Cheminformatics: Open Babel, RDKit

Docking: AutoDock Vina

Environment: Ubuntu WSL2, Python 3.10+, Jupyter Notebook

