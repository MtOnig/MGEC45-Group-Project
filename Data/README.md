# General Dataset Overview

Unit of observation: Player overall season data
Leagues: Top 5 European leagues (Premier League (England), Bundesliga (Germany), La liga (Spain), Serie A (Italy), Ligue 1 (France))
Seasons covered: 2017–2024
Position focus: Midfielders
Intended use:
* econometric modelling
* residual-based ranking
* multi-metric performance scoring
* player comparison & benchmarking
* Power BI visualization

This dataset serves as the single source of truth for all results reported in the written report and dashboard.

## Datasets

### **1. MGEC45_Final_Clean_Data.csv**
This is the **final cleaned base dataset** used as input for all modelling and scoring procedures.

**Contents include:**
- Player identifiers (Player, Team, Season, Nation)
- Playing time variables (Minutes, Matches, 90s)
- Core performance metrics from FBref (defensive actions, progression, passing, creativity)
- Variables used as regressors in all econometric models

---

### **2. Raw_Score_Data.csv**
This dataset contains the **multi-metric scoring system outputs** derived from the base dataset.

**Includes:**
- Standardized performance scores:
  - Defensive score
  - Progression score
  - On-ball security score
  - Creativity score
- Percentile rankings for each score
- Player-level comparisons used in ranking and similarity analysis

This file was used to:
- create leaderboards
- identify players outperforming Caicedo in multiple dimensions
- compute similarity distances

---

### **3. Transfer_Value_Expected_vs_Predicted.csv**
This dataset contains the **market value evaluation outputs** from the valuation regression.

**Includes:**
- Actual market values (Transfermarkt)
- Predicted market values from the regression model
- Market value residuals (actual − predicted)
- Inputs used to assess over- and undervaluation

This file underpins:
- the valuation analysis
- Caicedo’s overvaluation estimate
- visualizations comparing expected vs actual value

---
### **4. Offensive_Defensive_Overall_residuals.csv**
This dataset contains residual outputs from the three performance regressions:

**Includes:**
- Defensive contribution residuals
- Offensive contribution residuals
- Overall impact (plus-minus) residuals

Used for:
- residual-based rankings
- leaderboard construction
- benchmarking Caicedo against other midfielders

This file isolates pure performance deviations from team and contextual effects.
---

## Relationship Between Datasets

The datasets follow this pipeline:

MGEC45_Final_Clean_Data.csv
        ↓
Performance Regression Models
        ↓
Offensive_Defensive_Overall_residuals.csv
        ↓
Raw_Score_Data.csv        Transfer_Value_Expected_vs_Predicted.csv
