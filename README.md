# NBA Player Salary Analysis

What factors most strongly influence NBA player salaries: college background, team-level salary investment, or draft position? Completed as a team project at Hult International Business School.

## Overview

The NBA is a multi-billion dollar industry where talent acquisition and salary allocation directly impact team performance and financial sustainability. This project joins three separate datasets — player biographical info, salary history, and team details — to answer strategic questions relevant to talent scouts, team managers, and college programs:

1. Which colleges produce the most successful (highest-paid) NBA players?
2. How do team salary spending strategies compare across the league?
3. Does draft position predict career earning potential?

## Approach

- **Data cleaning & joining:** Merged player biographical data (1,928 players), 25 years of salary records (11,327 rows, 2000–2025), and team details (25 teams) via `person_id` and `team_id` joins.
- **Exploratory analysis:** Examined salary distribution, dataset structure, and data quality (missing values, duplicates) before analysis.
- **College pipeline analysis:** Counted and ranked NBA players and average salary by originating university.
- **Team spending analysis:** Computed average player salary per team to compare payroll strategies.
- **Draft position analysis:** Modeled the relationship between draft pick number/round and average career salary.

## Key Findings

- **Salary distribution is highly right-skewed** — a small number of star players earn exceptionally high salaries, meaning league-wide averages can be misleading without distributional analysis (median, percentiles).
- **Draft position matters, but with high variance** — earlier picks (especially lottery picks) have higher expected salaries, but several later-round picks achieve salaries comparable to first-round players.
- **A small number of colleges are reliable talent pipelines** — Duke, Kentucky, and Kansas produced the most NBA players in the dataset (282, 271, and 190 respectively).
- **Team payroll strategies vary significantly** — the Lakers, Bucks, and Bulls had the highest average player salaries, reflecting different roster construction philosophies (star-heavy vs. balanced payrolls).

## Repository Contents

- `nba_salary_analysis.ipynb` — full analysis: data cleaning, joins, exploratory visualizations, and business insights

## Tools

Python (pandas, numpy, matplotlib, seaborn, PIL), Jupyter Notebook

## Team

Alejandro Lopez, Luca Gillich, Milica Kurtovic, Sven Schaaser, Theodora Omiridou
