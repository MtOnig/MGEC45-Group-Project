# Moises Caicedo valutaion analysis - MGEC45 Project

A statistical evaluation of whether Moisés Caicedo’s £115M transfer fee reflects his measurable on-pitch performance, using econometric modelling, multi-metric scoring, and market value prediction.


## Project Summary
This project analyzes midfielder performance across Europe’s top 5 leagues (2017–2024) to assess whether Moisés Caicedo’s 2023 transfer to Chelsea was economically justified.

Using R, we built four key regression models:
- Defensive Contribution Model (xGA/90 with defensive actions + team fixed effects)
- Offensive Contribution Model (xG/90 with key passes, progressive actions + fixed effects)
- Overall Impact Model (+/- per 90 as a measure of team performance contribution)
- Market Value Regression (predicting player valuation using performance contribution + fixed effects)

We complemented these models with a multi-metric scoring system, percentile rankings, and similarity analysis to benchmark Caicedo against other elite midfielders.

## My Individual Contributions
As part of this MGEC45 group project, our team collectively developed the analytical framework used to evaluate Moisés Caicedo’s transfer valuation. Together, we:
- built the four core regression models (defensive, offensive, overall impact, market value)
- conducted residual analysis and ranking of ~1,000 midfielders
- generated leaderboards and comparison tables across performance metrics
- benchmarked Caicedo against three midfielders: Declan Rice, N’Golo Kanté, and Carlos Baleba
- prepared findings for our written report and class presentation

My individual contributions focused specifically on the statistical analysis of Caicedo during the 2022-2023 season (the year before his move) and the creation of tools powering the final evaluation, including:
- analyzing Caicedo’s performance across all models and extracting his detailed residual, percentile, and ranking results
- engineering the full multi-metric scoring system (defense, progression, creativity, on-ball security), including z-scores and percentile transformation
- developing the similarity-matching method used to identify Caicedo’s closest statistical comparators
- preparing all export-ready datasets used for our interactive Power BI dashboard, including player lookup tables, percentile outputs, and cleaned scoring data
- Developoing the PowerBI report and Dashboard.
- resolving data-cleaning issues such as name mismatches, missing values, and per-90 normalization

This README provides a high-level view of the project. A separate documentation file will be added to explain each component,models, scoring system, datasets, and dashboard in more detail.

##  Main Report

The full written analysis, including methodology, results, discussion, and personal reflection, is available here:

➡️ **[Caicedo Transfer Valuation Report (PDF)](./Final_Report_and_Reflection.pdf)**

This report evaluates whether Moisés Caicedo’s £115M transfer fee aligns with his measurable on-pitch performance using econometric residual analysis, composite scoring methods, and interactive visualizations. It also includes my personal reflection on the process and things I think we could do better going forward.
