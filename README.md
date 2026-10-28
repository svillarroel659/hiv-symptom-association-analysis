# HIV Symptom Association Analysis

## Overview

This project examines the relationships among fatigue, weakness, and treatment outcomes in people living with HIV.

The goal was to determine whether the intervention was associated with changes in fatigue, weakness, or both.

## Data

The analysis used data from a randomized clinical trial of 609 participants. After incomplete observations were removed, the final dataset contained 1,343 symptom reports.

The main variables were:

- Fatigue severity
- Weakness severity
- Treatment group

## Methods

The analysis was conducted in R using:

- Multinomial logistic regression
- Ordinal logistic regression
- Log-linear modeling
- Likelihood-ratio tests
- AIC and BIC for model comparison

## Key Findings

- Fatigue and weakness were strongly associated.
- Treatment was associated with lower fatigue after accounting for weakness.
- Fatigue was the strongest predictor of weakness.
- Treatment did not show a clear direct effect on weakness after fatigue was considered.
- The log-linear analysis supported all pairwise relationships without requiring a three-way interaction.

Overall, treatment was associated with lower fatigue severity, while its independent association with weakness was less clear after accounting for fatigue. Further analysis would be needed to establish whether fatigue mediates the treatment's effect on weakness.

## Tools

- R
- R Markdown
- `nnet`
- `MASS`

## Data Availability

The dataset used in this project was provided for academic use and cannot be shared publicly. Therefore, the data file is not included in this repository.

## Limitations

The dataset contained repeated symptom reports from the same participants, but observations were treated as independent in this analysis. The models also did not adjust for additional clinical or demographic variables.

Future analysis could use longitudinal methods to account for repeated measurements and investigate treatment effects more directly.
