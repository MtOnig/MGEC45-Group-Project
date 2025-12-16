# Dataset Overview
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

# Variable Groups

The dataset contains several categories of variables:

1. Player Identifiers
* Player
* Team
* Season
* Nation
Used for filtering, grouping, and benchmarking players (e.g., Caicedo vs Rice, Kanté, Baleba).

2. Playing Time & Context
* Min, MP, Starts, 90s played
* Team indicators (used for fixed effects)
These variables are used for sample restrictions and regression controls.

3. Performance Metrics (Model Inputs)
Used as regressors across the defensive, offensive, and overall impact models, including:
Defensive actions: Tkl+Int, Recov/90
Ball progression: PrgC, Prg Passes
Creativity: Key Passes, xG when on/90
Possession & control: Passes Cmp%, Touches/90

4. Regression Model Outputs
* Generated from the four core econometric models:
* Defensive_Contribution_resid
* Offensive_Contribution_resid
* Overall_impact_resid
* predicted_value (market value model)
* Residual (actual − predicted market value)
These variables are used for ranking players, identifying over/undervaluation, and producing residual distributions.

