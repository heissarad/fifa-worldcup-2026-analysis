# Data

This folder contains the datasets used to answer the four research questions in the FIFA World Cup 2026 analysis.

## Dataset Files

### q1_player_shooting_raw.csv

This dataset contains player shooting statistics and is used for Question 1, which compares shots on target per 90 minutes for forwards from knockout-stage teams and group-stage teams.

Important columns used in the analysis include:

- `Player` – player name
- `Pos` – player position
- `Squad` – national team
- `90s` – number of 90-minute periods played
- `Sh` – total shots
- `SoT` – shots on target
- `SoT%` – percentage of shots that were on target
- `Sh/90` – shots per 90 minutes
- `SoT/90` – shots on target per 90 minutes

The analysis filters the dataset to include forwards before comparing the two tournament-stage groups.

### q2_goalkeeper_raw.csv

This dataset contains team goalkeeper statistics and is used for Question 2.

Important columns include:

- `Squad` – national team
- `MP` – matches played
- `Min` – minutes played
- `GA` – goals against
- `SoTA` – shots on target against
- `Saves` – total goalkeeper saves
- `SavePct` – save percentage
- `CS` – clean sheets

Saves per match are calculated using the number of saves and matches played.

### q3_ball_possession_raw.csv

This dataset contains team-level performance statistics and is used for Question 3 to compare ball possession between knockout-stage and group-stage teams.

Important columns include:

- `Squad` – national team
- `Poss` – average ball possession percentage
- `MP` – matches played
- `Min` – minutes played
- `Gls` – goals
- `Ast` – assists

For the analysis, the `Poss` column is renamed to `Possession`.

### q4_team_shooting_raw.csv

This dataset contains team shooting statistics and is used for Question 4.

The main columns are:

- `Squad` – national team
- `Sh` – total shots
- `shots_per_match` – average number of shots taken per match
- `stage` – identifies whether the team reached the knockout stage or was eliminated in the group stage

## Tournament Stage Classification

The analyses compare two groups:

- `knockout` – teams that advanced to the knockout stage
- `group_stage` – teams that were eliminated in the group stage

Tournament-stage classification is added during the analysis where it is not already included in the dataset.

## Data Preparation

The datasets are prepared in their corresponding Jupyter Notebooks before statistical analysis. Depending on the research question, this includes selecting relevant columns, filtering players by position, cleaning team names, creating tournament-stage groups, calculating per-match statistics, and selecting samples for comparison.

See the [`notebooks`](../notebooks/) folder for the complete analysis.
