# PC-Ir-ML: Machine Learning Models for Predicting Redox Potentials of Iridium(III) Photocatalysts

This repository accompanies the paper:  
**“Machine Learning-Assisted Prediction of Ground- and Excited-State Redox Potentials in Iridium(III) Photocatalysts”**  
X. Li, L. Fan, C. Xiong, W. Nie, Y. Dong, B. Zhu, W. Guan, *Angew. Chem. Int. Ed.*, 2025, e202517393.  
[https://doi.org/10.1002/anie.202517393](https://doi.org/10.1002/anie.202517393)

---

## Overview

This repository contains the machine learning models, datasets, and feature-generation scripts developed for predicting the **ground- and excited-state redox potentials** of Ir(III) photocatalysts.  
It includes all code used for model selection, optimization, and final model evaluation, as well as representative data and descriptor-generation workflows.

---

## Repository Structure

### **Model Folders**
Each of the six model folders includes code and trained models used in the study.

- **Gox/** — Ground-state oxidation potential model  
- **Gred/** — Ground-state reduction potential model  
- **Eox/** — Excited-state oxidation potential model  
- **Ered/** — Excited-state reduction potential model  
- **Model_G/** — Generalized ground-state model  
- **Model_E/** — Generalized excited-state model  

Each folder contains:
- `model_selection.ipynb` — algorithm and hyperparameter comparison  
- `model_optimization.ipynb` — optimization and fine-tuning process  
- `final_model.joblib` — trained model for direct inference  

---

### **data/**
Contains example data and molecular identifiers.

- `smiles.csv` — SMILES strings of all studied complexes  
- `sample.xlsx` — Eight representative examples including molecular names, redox potentials, and selected feature values  

> *Note:* Only representative examples are provided at this stage.  
> The complete numerical datasets (all features and target values) will be released after the completion of ongoing related studies.

---

### **Descriptor/**
Contains scripts for feature extraction and descriptor calculation.

- `Extraction.py` — Workflow for calculating PhysOrg-type descriptors  
- `Multiwfn.py` — Interface for quantum-chemical descriptor extraction via Multiwfn  
- `RDKit-desc.ipynb` — Example notebook for RDKit descriptor generation  

These scripts reproduce the descriptor-generation procedures described in the paper and can be adapted for other photocatalytic systems.

---

## How to Use

1. Clone or download this repository.  
2. Install the required Python packages (`requirements.txt`).  
3. Navigate to the desired model or descriptor folder.  
4. Use the Jupyter notebooks or Python scripts to:
   - Generate molecular descriptors from SMILES or SDF files.  
   - Perform model selection, optimization, and evaluation as described in the publication.  

---

## Citation

If you use or adapt any part of this repository (data, scripts, or models), please cite:

> X. Li, L. Fan, C. Xiong, W. Nie, Y. Dong, B. Zhu, W. Guan,  
> *Machine Learning-Assisted Prediction of Ground- and Excited-State Redox Potentials in Iridium(III) Photocatalysts*,  
> *Angew. Chem. Int. Ed.*, 2025, e202517393.  
> [https://doi.org/10.1002/anie.202517393](https://doi.org/10.1002/anie.202517393)

---

## License and Contact

All code and data are released for academic and non-commercial use.  

---

*© 2025 X. Li et al. All rights reserved.*
