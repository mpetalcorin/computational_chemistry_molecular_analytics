
# GROMACS, QSAR, OpenEye and Molecular Docking Demo

This repository contains a computational chemistry notebook for drug discovery. It demonstrates, using simulated data, how scientists can use computer-based methods to study molecules, predict drug-like behaviour, and prioritise compounds for testing.

The project is designed for learning purposes. It does not require paid commercial software. The notebook uses simulated molecular values that are kept within realistic ranges commonly seen in computational drug discovery studies.

<img width="1536" height="1024" alt="GROMACS Molecular Dynamics" src="https://github.com/user-attachments/assets/b72c29d6-9e33-4265-9f64-396e7f35647b" />

## Project Goal

The goal of this project is to show how different computational chemistry methods work together in a modern drug discovery workflow.

The notebook demonstrates how to:

- Simulate a compound library.
- Predict molecular activity using QSAR.
- Analyse docking-like scores.
- Build a virtual screening funnel.
- Simulate GROMACS-style molecular dynamics results.
- Analyse quantum-mechanics-style molecular descriptors.
- Simulate FEP-style lead optimisation.
- Create Spotfire-style SAR tables and heatmaps.
- Simulate OpenEye-style molecular shape and electrostatic similarity.
- Combine all results into a final compound priority ranking.

---

## Explanation of the Main Topics

### 1. GROMACS

GROMACS is software used to simulate how molecules move, making a molecular movie. Scientists can watch how a protein, a drug molecule, water, and ions move inside a computer simulation.

In this project, GROMACS-style outputs are simulated, including:

- RMSD, which measures how much a protein structure moves.
- RMSF, which shows which protein regions are flexible.
- Radius of gyration, which shows whether the protein stays compact.
- Hydrogen bonds, which show whether the drug stays attached.
- Ligand-pocket distance, which shows whether the drug remains inside the binding site.

---

### 2. Molecular Dynamics

Molecular dynamics is the method used to study molecular movement over time. Proteins are not frozen objects but are able to bend, breathe, open, close, and change shape.

In drug discovery, molecular dynamics helps answer questions such as:

- Does the drug stay bound to the protein?
- Does the protein remain stable?
- Does the binding pocket change shape?
- Does the ligand drift away?

---

### 3. Docking

Docking predicts how a drug-like molecule may fit into a protein. A common analogy is a key fitting into a lock. The protein is the lock, and the drug molecule is the key.

Docking gives a docking score. A more negative docking score usually suggests better predicted binding, but docking is only a prediction. It must be checked with other methods and eventually tested in the lab.

---

### 4. Virtual Screening

Virtual screening means testing many molecules on a computer before testing them experimentally.

Instead of testing thousands or millions of compounds in the lab, scientists use computer filters to shortlist the most promising molecules.

This project uses a simple virtual screening funnel based on:

- Docking score.
- Molecular similarity.
- Predicted activity.
- ADMET quality.
- FEP-style improvement.

---

### 5. Quantum Mechanics

Quantum mechanics studies molecules at the electron level. It helps scientists understand bonds, charges, electron movement, and chemical reactivity.

In this notebook, quantum-mechanics-style descriptors include:

- HOMO energy.
- LUMO energy.
- HOMO-LUMO gap.
- Dipole moment.

These values help describe electronic features of molecules.

---

### 6. FEP

FEP means free energy perturbation. It is used to estimate whether a small chemical change may improve or weaken drug binding.

For example, a chemist may ask:

What happens if I replace one chemical group with another?

FEP helps predict whether that change may make the compound better before it is synthesised.

---

### 7. QSAR

QSAR means quantitative structure-activity relationship. In simple terms, QSAR predicts what a molecule may do based on its structure.

The computer converts each molecule into numbers, such as descriptors and fingerprints. A machine learning model then learns how molecular features relate to biological activity.

In this notebook, QSAR is used to:

- Classify compounds as active or inactive.
- Predict pIC50 values.
- Identify important molecular features.

---

### 8. Spotfire-Style SAR Analytics

Spotfire is commonly used in pharma for visualising compound data. It helps scientists explore patterns in structure-activity relationships, often called SAR.

This project creates Spotfire-style outputs such as:

- SAR heatmaps.
- Potency buckets.
- Compound decision tables.
- Drug discovery triage tables.

If the term “Sportfire” was intended, it may refer to Spotfire or a specific QSAR-related platform.

---

### 9. OpenEye-Style Molecular Similarity

OpenEye is a professional computational chemistry toolkit used for molecular design and comparison.

This notebook simulates OpenEye-style ideas such as:

- Molecular shape similarity.
- Electrostatic similarity.
- Combined molecular similarity.
- Ligand-based prioritisation.

The aim is to show how molecules can be compared based on 3D shape and charge-like properties.

---

## Files in This Repository

| File | Description |
|---|---|
| `computational_chemistry_molecular_analytics.ipynb` | Main Jupyter notebook containing the full analysis. |
| `simulated_molecular_analytics_dataset.csv` | Simulated molecular dataset generated by the notebook. |
| `final_prioritised_compounds.csv` | Final ranked compounds selected by the integrated decision engine. |
| `figures/` | Folder containing generated plots and visualisations. |
| `README.md` | This file. |

---

## How to Run the Notebook

Create a clean Python environment:

```bash
conda create -n compchem-demo python=3.11 pandas numpy matplotlib scikit-learn jupyterlab -y
conda activate compchem-demo
jupyter lab
```

Then open:

```text
computational_chemistry_molecular_analytics.ipynb
```

Run the notebook from top to bottom.

---

## Required Python Packages

The notebook uses:

```text
numpy
pandas
matplotlib
scikit-learn
jupyterlab
```

Optional packages can be added later for real molecular work:

```text
rdkit
mdtraj
nglview
openmm
deepchem
xgboost
shap
```

---

## What the Notebook Produces

The notebook produces:

- Molecular descriptor tables.
- Docking-like analysis.
- Virtual screening funnel.
- Molecular dynamics-style plots.
- RMSD and RMSF figures.
- Quantum descriptor plots.
- FEP-style optimisation plots.
- QSAR model performance metrics.
- ROC and precision-recall curves.
- Predicted versus observed pIC50 plots.
- Feature importance charts.
- PCA chemical-space maps.
- SAR heatmaps.
- OpenEye-style similarity plots.
- Final compound ranking table.

---

## Example Scientific Interpretation

A strong candidate compound in this workflow should have:

- High predicted potency.
- Favourable docking score.
- Favourable FEP-style relative free energy.
- Good shape and electrostatic similarity.
- Acceptable ADMET profile.
- Stable MD-style behaviour.
- Good integrated priority score.

The final ranked compounds are not real experimental drug candidates. They are simulated examples designed to demonstrate how computational drug discovery decisions are made.

---

## Why This Project Is Useful

This project is useful because it shows how computational chemistry methods connect to real drug discovery decisions.

It demonstrates that molecular modelling is not only about running software. It is about asking better scientific questions:

- Which compounds should we test first?
- Which compounds may bind better?
- Which compounds may be unstable?
- Which compounds may have ADMET risks?
- Which chemical series looks most promising?
- Which predictions need experimental validation?

---

## Important Disclaimer

All data in this project are simulated. The values are designed to be realistic but are not experimental measurements. The notebook should be used for education, demonstration, and learning preparation only.

It should not be used to make real clinical, regulatory, or experimental decisions without proper experimental validation.

---

## Scientific References

The notebook is conceptually benchmarked against scientific journal literature-indexed computational drug discovery references, including studies on GROMACS, molecular dynamics, docking, virtual screening, FEP, QSAR, molecular shape similarity, and SAR visualisation.

Key references include:

- Hess B, Kutzner C, van der Spoel D, Lindahl E. GROMACS 4: algorithms for highly efficient, load-balanced, and scalable molecular simulation. *Journal of Chemical Theory and Computation*. 2008.
- Trott O, Olson AJ. AutoDock Vina: improving the speed and accuracy of docking with a new scoring function. *Journal of Computational Chemistry*. 2010.
- Kitchen DB, Decornez H, Furr JR, Bajorath J. Docking and scoring in virtual screening for drug discovery. *Nature Reviews Drug Discovery*. 2004.
- Wang L, Wu Y, Deng Y, et al. Protein-ligand binding free energy calculations with FEP. *Chemical Reviews*. 2019.
- Carracedo-Reboredo P, Liñares-Blanco J, Rodríguez-Fernández N, et al. A review on machine learning approaches and trends in drug discovery. *Computational and Structural Biotechnology Journal*. 2021.
- Arodola OA, Soliman MES. Quantum mechanics implementation in drug-design workflows. *Drug Design, Development and Therapy*. 2017.
- Nicholls A, McGaughey GB, Sheridan RP, et al. Molecular shape and medicinal chemistry: a perspective. *Journal of Medicinal Chemistry*. 2010.
- Agrafiotis DK, Shemanarev M, Connolly PJ, Farnum M, Lobanov VS. SAR maps: a new SAR visualization technique for medicinal chemists. *Journal of Medicinal Chemistry*. 2007.

---

## Author

Mark I.R. Petalcorin, PhD

This repository was prepared as a computational chemistry and AI-enabled drug discovery project.

