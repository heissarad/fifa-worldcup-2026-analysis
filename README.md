# FIFA World Cup 2026 Analysis

## Project Overview

This project analyses FIFA World Cup 2026 data to explore whether selected football performance statistics differ between teams that advanced to the knockout stage and teams that were eliminated in the group stage.

The analysis focuses on four areas: forwards' shooting performance, goalkeeper saves, team ball possession, and team shooting performance. Python and Jupyter Notebook were used to prepare, analyse, and compare the data.

## Research Questions

### Q1: Forwards – Shots on Target

On average, how many shots on target per 90 minutes did forwards register, and do forwards on knockout teams register more shots on target per 90 minutes than forwards eliminated in the group stage?

### Q2: Goalkeeper Saves

On average, how many saves does a team's goalkeeper make per match during the FIFA World Cup 2026? Is there a significant difference between teams eliminated in the group stage versus teams that advanced to the knockout stage?

### Q3: Ball Possession

Is there a significant difference in average ball possession (%) between FIFA World Cup 2026 teams that reached the knockout stage versus those eliminated in the group stage?

### Q4: Team Shots

On average, how many shots does a team take per match at the FIFA World Cup 2026? Is there a significant difference between teams that advanced to the knockout stage and those eliminated in the group stage?

## Repository Structure

```text
fifa-worldcup-2026-analysis/
│
├── data/
│   ├── q1_player_shooting_raw.csv
│   ├── q2_goalkeeper_raw.csv
│   ├── q3_ball_possession_raw.csv
│   ├── q4_team_shooting_raw.csv
│   └── README.md
│
├── notebooks/
│   ├── q1_shooting_analysis.ipynb
│   ├── q2_goalkeeper_saves_analysis.ipynb
│   ├── q3_possession_analysis.ipynb
│   ├── q4_team_shooting_analysis.ipynb
│   └── README.md
│
└── README.md
```

## Analysis Approach

The analysis compares two groups:

- Teams that advanced to the knockout stage
- Teams that were eliminated in the group stage

For each research question, the relevant data was selected and prepared before calculating descriptive statistics such as averages.

Statistical tests were then used to examine whether the differences observed between the two groups were statistically significant. A significance level of **0.05** was used to interpret the statistical results.

## Summary of Results

| Question | Group Stage | Knockout Stage | p-value | Result |
|---|---:|---:|---:|---|
| Q1 – Shots on target per 90 | 0.714 | 0.590 | 0.5903 | No significant difference |
| Q2 – Goalkeeper saves per match | 3.042 | 2.435 | 0.3451 | No significant difference |
| Q3 – Ball possession | 44.66% | 52.53% | 0.0891 | No significant difference |
| Q4 – Shots per match | 10.168 | 12.398 | 0.0984 | No significant difference |

Based on the statistical tests used in the notebooks, none of the four comparisons produced a p-value below the **0.05 significance level**. Therefore, the analyses did not find sufficient statistical evidence of a significant difference between the compared groups.

## Tools and Libraries

The project uses:

- **Python** – used to perform the data analysis
- **Jupyter Notebook** – used to write and run the analysis
- **Pandas** – used for loading, cleaning, filtering, and analysing the datasets
- **SciPy** – used to perform the statistical tests
- **Requests** – used in the project for retrieving web data
- **BeautifulSoup** – used for processing data obtained from web pages

## Data and Notebooks

More information about the datasets and variables used in this project is available in the [`data`](data/) folder.

The analysis and statistical testing for each research question can be found in the [`notebooks`](notebooks/) folder.
