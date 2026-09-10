# Notebooks

This folder contains the Jupyter Notebooks used to answer the four research questions in the FIFA World Cup 2026 analysis.

Each notebook contains the data preparation, calculations, statistical testing, and interpretation for its corresponding research question.

## q1_shooting_analysis.ipynb

### Question 1: Forwards' Shots on Target

This notebook investigates:

> On average, how many shots on target per 90 minutes did forwards register, and do forwards on knockout teams register more shots on target per 90 minutes than forwards eliminated in the group stage?

The analysis includes:

- Loading the player shooting dataset
- Selecting the relevant shooting statistics
- Filtering players to include forwards
- Classifying players based on whether their team reached the knockout stage or was eliminated in the group stage
- Comparing shots on target per 90 minutes between the two groups
- Performing a statistical test to determine whether the difference is significant

### Result

- Group-stage forwards: **0.714 shots on target per 90**
- Knockout-stage forwards: **0.590 shots on target per 90**
- p-value: **0.5903**

The result was not statistically significant at the 0.05 significance level.

---

## q2_goalkeeper_saves_analysis.ipynb

### Question 2: Goalkeeper Saves

This notebook investigates:

> On average, how many saves does a team's goalkeeper make per match during the FIFA World Cup 2026? Is there a significant difference between teams eliminated in the group stage versus teams that advanced to the knockout stage?

The analysis includes:

- Loading and preparing the goalkeeper dataset
- Using goalkeeper saves and matches played
- Calculating saves per match
- Classifying teams into knockout-stage and group-stage groups
- Calculating the overall average saves per match
- Comparing the two groups
- Performing a statistical test to determine whether the difference is significant

### Result

- Overall average: **2.597 saves per match**
- Group-stage teams: **3.042 saves per match**
- Knockout-stage teams: **2.435 saves per match**
- p-value: **0.3451**

The result was not statistically significant at the 0.05 significance level.

---

## q3_possession_analysis.ipynb

### Question 3: Ball Possession

This notebook investigates:

> Is there a significant difference in average ball possession (%) between FIFA World Cup 2026 teams that reached the knockout stage versus those eliminated in the group stage?

The analysis includes:

- Loading the team possession dataset
- Selecting the relevant team and possession data
- Renaming the possession variable for the analysis
- Classifying teams according to tournament progression
- Comparing average possession between the two groups
- Performing a statistical test to determine whether the difference is significant

### Result

- Group-stage teams: **44.66% average possession**
- Knockout-stage teams: **52.53% average possession**
- p-value: **0.0891**

Knockout-stage teams had higher average possession in the analysed sample, but the difference was not statistically significant at the 0.05 significance level.

---

## q4_team_shooting_analysis.ipynb

### Question 4: Team Shots

This notebook investigates:

> On average, how many shots does a team take per match at the FIFA World Cup 2026? Is there a significant difference between teams that advanced to the knockout stage and those eliminated in the group stage?

The analysis includes:

- Loading the team shooting dataset
- Selecting team shooting and tournament-stage information
- Calculating the overall average shots per match
- Separating teams into knockout-stage and group-stage groups
- Comparing average shots per match between the groups
- Performing a statistical test to determine whether the difference is significant

### Result

- Overall average: **11.803 shots per match**
- Group-stage teams: **10.168 shots per match**
- Knockout-stage teams: **12.398 shots per match**
- p-value: **0.0984**

Knockout-stage teams had a higher average number of shots per match in the analysed sample, but the difference was not statistically significant at the 0.05 significance level.

---

## Statistical Significance

A significance level of **0.05** is used throughout the analysis.

A p-value below 0.05 is considered evidence of a statistically significant difference between the groups. A p-value above 0.05 means there is not enough statistical evidence to conclude that the groups are significantly different.

In these analyses, all four p-values were above 0.05, so none of the observed group differences were statistically significant.
