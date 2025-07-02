# AOBp_Ben-Zeev_et_al_2025
Files for the "Neighbor sensing through rhizodeposits in sorghum affects plant physiology and productivity" Paper

# Neighbor Sensing in Sorghum: Experimental Data and Metadata

This repository contains all datasets, metadata, and documentation necessary to reproduce the analyses and results presented in the manuscript:


---

## Repository Contents

### 📂 Data Files

| Filename | Description |
|----------|-------------|
| `Ben_Zeev_etal_EXP1.csv` | Dataset for Experiment 1: Performance of sorghum PI lines under factorial combinations of drought and competition. Includes biomass, leaf area, height, stomatal conductance, and quantum yield. |
| `Ben Zeev et al 2025 EXP2.csv` | Dataset for Experiment 2 (general measurements): Performance of PI lines under leachate and competition treatments, including shoot/root biomass, shoot:root ratio, and digital root architecture traits. |
| `CompLeach_Licor6800summary.csv` | Gas exchange measurements (subset of EXP2 plants): Includes steady-state assimilation rate, stomatal conductance, instantaneous WUE, and transpiration rate. |
| `BenZeev_MetadataTable.csv` | A three-column metadata file detailing all variables used in the paper, including units and interpretation. Covers categorical factors (Genotype, Treatment, etc.) and all measured traits. |

---

## 📋 Experimental Overview

### EXP1 — Competition × Drought
- **Design:** Full factorial (2 Competition × 2 Drought) applied to sorghum PI lines.
- **Measurements:** Dry weight, leaf area, plant height, stomatal conductance, quantum yield.
- **Goal:** Determine whether root-mediated interactions modulate genotype responses to drought and competition.

### EXP2 — Leachate Transfer
- **Design:** PI lines grown with/without competition or leachate derived from neighbors.
- **Measurements:** Shoot and root biomass, shoot:root ratio, leaf area, and root traits from image analysis.
- **Gas Exchange Subset:** Selected plants measured for assimilation, stomatal conductance, iWUE, and transpiration using LICOR 6800.

---

## 📑 Metadata Table

Each variable in the dataset is documented in the metadata file (`BenZeev_MetadataTable.csv`) with the following columns:
- **Variable Name** – matches the column name in the CSVs
- **Unit** – standardized scientific units (e.g., g, cm², mol m⁻² s⁻¹)
- **Interpretation** – clear explanation of the variable’s meaning and relevance

All experimental factors (e.g. `Genotype`, `Block`, `Drought`, `Treat`, `Comp`) are included as well, to ensure clarity in replication or reuse.

---

## 🔁 Reproducibility

All statistical analyses were conducted in R using `lmerTest`, `lme4`, and `car`. Separate scripts are used to:
- Fit linear mixed models for EXP1 and EXP2
- Run Type III ANOVA with Satterthwaite degrees of freedom
- Analyze gas exchange with fixed-effect models (due to limited replication)

Please cite this repository alongside the manuscript if using the data.

---

## 📞 Contact

For questions about the data or manuscript, contact:

**Shiran Ben Zeev**  

Email: shiranbz@gmail.com]  
