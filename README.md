# ASHA Survey Methodology Analysis

This repository contains the full analysis for the American Speech-Language-Hearing Association (ASHA) survey methodology project. The goal of this project is to evaluate survey design decisions—specifically postcard reminders and survey mode—and quantify their effects on response behavior.

## Project Overview

This project addresses two core methodological questions:

1. Postcard Experiment (2025 SLP Health Care Survey)
   - Does sending postcard reminders increase response rates?
   - What is the marginal effect of the first and second postcard?
   - Are there short-term response boosts following postcard mailings?

2. Survey Mode Experiment (2024 & 2025 Surveys)
   - How does survey mode (Postal Mail vs. SurveyMonkey) affect response rates?
   - Do subgroups (age, employment, region, facility) respond differently by mode?
   - Does survey mode introduce composition bias?

The analysis follows a survey methodology framework, emphasizing:
- Treatment by indication
- Policy estimands
- Nonresponse behavior
- Mode effects and Total Survey Error (TSE)


## Data Description

The project uses two primary datasets:

1. 2025 SLP Health Care Survey
- Sample size: ~15,000 SLPs
- Web sample used for postcard experiment: 9,947
- Response rate: ~18.6%
- Includes:
  - Postcard treatment groups (0, 1, 2 postcards)
  - Response timing (start and end date)

2. 2024 SLP Schools Survey
- Sample size: 15,000 SLPs
- Mixed-mode design (Mail vs. Web)
- Includes subgroup variables:
  - Age
  - Employment status
  - Facility type
  - Region

## Methods

Postcard Experiment
- Policy estimand framework to address treatment by indication
- Decomposition using conditional probabilities
- Five component response rates (RR1–RR5)
- Bootstrap inference (B = 2000)

Short-Term Effects (Q4)
- Daily response time series
- Pre/post window comparison (7-day windows)
- Difference-in-Differences (DiD) estimation

Survey Mode Analysis
- Response rate comparisons (Mail vs. Web)
- Pearson chi-square tests within subgroups
- Logistic regression models (main + interaction)
- Likelihood Ratio Tests (LRT)


## Key Findings

Postcard Experiment
- First postcard increases response rate by ~1.26 percentage points (statistically significant)
- Second postcard provides no additional meaningful benefit
- Short-term increases exist but are modest compared to email reminders

Survey Mode
- Postal mail consistently outperforms web
- Web reduces response odds by ~37%
- Strongest effects observed in older respondents and part-time employees
- Mode effects are consistent across regions
- Limited evidence of composition bias


## Reproducibility

1. Clone the repository:
git clone https://github.com/Sagnik-Chakravarty/ASHA.git

2. Open R or RStudio

3. Install required packages:
install.packages(c("tidyverse", "survey", "broom", "ggplot2"))

## Authors

- **Sagnik Chakravarty**  
  University of Maryland (JPSM)  
  Email: sagnikch@umd.edu  

- **Ruisi Ma**  
  University of Michigan  
  Email: ruisima@umich.edu  

- **Yuchen Ding**  
  University of Michigan  
  Email: yuchennn@umich.edu  

- **Feiran Ge**  
  University of Michigan  
  Email: aptx@umich.edu  
