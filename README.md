# Distill2MD-Interfaces

Companion repository for the paper:

**Distilling an atomistic foundation model is all you need for large-scale molecular dynamics of semiconductor interfaces**

This repository provides D00 student potentials distilled from EquiformerV3 (EqV3), D100 potentials trained on DFT reference labels, and their corresponding training datasets.

| System | Potential | Files |
| --- | --- | --- |
| BAs/GaN | NEP | [BAs-GaN](BAs-GaN/) |
| Cu–diamond | ACE | [Cu-diamond](Cu-diamond/) |
| SiC/a-C/SiC | NEP | [SiC-aC-SiC](SiC-aC-SiC/) |

Each system includes three models per strategy (D00 and D100), with training seeds `20260901`, `20260902` and `20260903`.

NEP potentials (`.txt`) are provided for GPUMD, and ACE potentials (`.yace`) for LAMMPS/PACE. Training data are supplied as compressed extended XYZ files for NEP and pandas pickle files for ACE.

D00 datasets: `train-eqv.xyz.gz` (NEP) and `train.pkl.gz` (ACE).

D100 datasets: `train-dft.xyz.gz` (NEP) and `train-dft.pkl.gz` (ACE).
