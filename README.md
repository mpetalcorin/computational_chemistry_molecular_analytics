# GROMACS QSAR OpenEye Molecular Docking

This repository contains a molecular analytics demonstration notebook covering:

- GROMACS-style molecular dynamics analytics
- Molecular dynamics trajectory outputs, including RMSD, RMSF, radius of gyration, hydrogen bonds, and ligand-pocket distance
- Docking and virtual screening
- Quantum mechanics-style molecular descriptors
- FEP-style lead optimisation
- QSAR modelling
- Spotfire-style SAR analytics
- OpenEye-style molecular shape and electrostatic similarity
- Integrated molecular decision-making for drug discovery

The notebook uses simulated literature-benchmarked molecular values and is intended for portfolio, training, and interview demonstration purposes.

## How to run

```bash
conda create -n compchem-demo python=3.11 pandas numpy matplotlib scikit-learn jupyterlab -y
conda activate compchem-demo
jupyter lab
```

Then open the notebook in JupyterLab.
