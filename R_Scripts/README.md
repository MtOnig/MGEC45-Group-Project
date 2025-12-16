# RMarkdown Analysis Files

This folder contains the core analytical notebooks used in the MGEC45 project Moisés Caicedo Valuation Analysis. The RMarkdown files document the full econometric workflow, from residual estimation to composite score construction, ensuring transparency and reproducibility.

---

## Files Overview

### MGEC45_ResidualCalculations_and_Analysis.Rmd

This file performs the **econometric residual analysis** used to evaluate Moisés Caicedo’s on-pitch performance relative to a baseline midfielder.

**Key components:**
- Regression-based performance models for:
  - Offensive contribution  
  - Defensive contribution  
  - Overall impact  
- Extraction of **player-level residuals** as measures of over- or under-performance relative to model expectations  
- Standardization and ranking of residuals across a sample of ~1,000 midfielders from Europe’s top 5 leagues  
- Identification of Caicedo’s percentile rankings within each performance dimension  

**Output:**
- Residual values used in the final dataset  
- Performance rankings and distributions referenced in the appendix (MR sections)  
- Analytical justification for relative performance claims in the final report  

---

### MGEC45_ScoreCalculations_and_Analysis.Rmd

This file constructs the **composite performance score** used to assess whether Caicedo’s £115M transfer fee aligns with his measurable output.

**Key components:**
- Integration of offensive, defensive, and overall residual metrics  
- Normalization and weighting of performance dimensions  
- Construction of a **multi-metric scoring system**  
- Final player rankings based on composite scores  
- Sensitivity checks on scoring methodology  

**Output:**
- Final performance scores for all midfielders  
- Caicedo’s relative standing within the full sample  
- Inputs used for Power BI visualizations and comparative analysis  

---

## How These Files Fit Into the Project
These RMarkdown files serve as the analytical backbone of the project:
- Outputs feed directly into the final cleaned dataset
- Results are summarized in the written report and appendices
- Derived metrics are visualized in the accompanying Power BI dashboard
