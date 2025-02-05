
# README: RMSD Analysis for DpaA Structures

## Overview
This report summarizes the structural comparison of **DpaA_AlphaFold** (predicted model) and **DpaA_Experimental** (experimental structure) using Root Mean Square Deviation (RMSD) analysis.

---

## 1. Global RMSD Analysis
- **Command Used**: `rms_cur DpaA_AlphaFold, DpaA_Experimental`
- **Result**:  
  - **Number of Atoms Aligned**: 1970  
  - **Global RMSD**: 0.460 Å  
  - **Estimated Similarity**: ~98–99%

The global RMSD is exceptionally low, indicating a very close match between the AlphaFold prediction and the experimental structure.

---

## 2. Regional RMSD Analysis (Residues 1–100)
- **Command Used**: `rms_cur DpaA_AlphaFold and resi 1-100, DpaA_Experimental and resi 1-100`
- **Result**:  
  - **Number of Atoms Aligned**: 802  
  - **Regional RMSD**: 0.968 Å  
  - **Estimated Similarity**: ~92–95%

The slightly higher RMSD for this region suggests some flexibility or modeling differences, but the structures are still highly similar.

---

## 3. Files Generated
- **Aligned Global Structures**:
  - `aligned_DpaA_AlphaFold.pdb`
  - `aligned_DpaA_Experimental.pdb`
- **Regionally Aligned Structures (Residues 1–100)**:
  - `region_1_100_AlphaFold.pdb`
  - `region_1_100_Experimental.pdb`
- **Log File**:
  - `rmsd_report.log`

---

## 4. Notes
- **Global Similarity**: The AlphaFold prediction is ~98–99% similar to the experimental structure globally.
- **Regional Similarity**: Residues 1–100 exhibit ~92–95% similarity, reflecting some localized structural differences.
- These results highlight the high accuracy of AlphaFold in predicting the DpaA structure.
- Further analysis, such as hydrogen bond comparisons and secondary structure visualization, is recommended to better understand the discrepancies.

