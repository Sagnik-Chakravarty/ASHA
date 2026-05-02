# ASHA Survey Methodology Analysis

This repository documents a survey methodology analysis for the American Speech-Language-Hearing Association (ASHA). The project evaluates survey design decisions related to postcard reminders, survey mode, response rates, nonresponse behavior, and subgroup variation.

## Repository Description

Survey methodology project evaluating ASHA response behavior, postcard reminder effects, and postal mail vs. web survey mode differences using response-rate analysis, bootstrap inference, logistic regression, and stakeholder-facing recommendations.

## Project Motivation

Professional association surveys depend on careful design choices about mode of contact, follow-up reminders, respondent burden, and subgroup coverage. This project analyzes ASHA survey data to evaluate which design choices improve response and where mode or follow-up strategies may create differences in respondent behavior.

The analysis is framed through survey methodology concepts including nonresponse error, mode effects, treatment by indication, policy estimands, and Total Survey Error.

## Research Questions

1. Do postcard reminders increase response rates?
2. What is the marginal effect of the first and second postcard reminder?
3. Are short-term response boosts visible after postcard mailings?
4. How does postal mail compare with web/SurveyMonkey administration?
5. Do mode effects vary by age, employment status, region, or facility type?
6. Does survey mode create evidence of composition differences across respondent groups?

## Data Context

The project uses ASHA survey files, including respondent records and full sample-frame records.

Main survey contexts:

- **2025 SLP Health Care Survey**
  - Approximate sample size: 15,000 SLPs
  - Web sample for postcard experiment: 9,947
  - Response timing and postcard treatment information

- **2024 SLP Schools Survey**
  - Approximate sample size: 15,000 SLPs
  - Mixed-mode design: postal mail vs. SurveyMonkey/web
  - Subgroup variables: age, employment status, facility type, and region

## Methods

### Postcard Reminder Analysis

- Policy estimand framework to address treatment by indication
- Sequential response-rate decomposition using conditional probabilities
- Component response rates for no-card, one-card, and two-card regimes
- Bootstrap inference for uncertainty estimation
- Short-term response timing analysis around postcard mailings

### Survey Mode Analysis

- Postal mail vs. web/SurveyMonkey response-rate comparison
- Subgroup response-rate analysis by age, employment, region, and facility type
- Pearson chi-square tests for mode-response association
- Logistic regression models for response propensity
- Interaction models and likelihood ratio tests for subgroup-specific mode effects

## Key Findings

### Postcard Experiment

- The first postcard increased response by approximately 1.2–1.3 percentage points.
- The second postcard showed little additional marginal benefit.
- Short-term response boosts were present but modest relative to other reminder strategies.

### Survey Mode

- Postal mail consistently outperformed web/SurveyMonkey administration.
- Web mode was associated with substantially lower response odds relative to postal mail.
- The strongest mode differences appeared among older respondents and part-time employees.
- Mode effects were broadly consistent across regions.
- Evidence of composition bias was limited, but subgroup response differences remain important for survey design.

## Repository Structure

```text
.
├── README.md
├── ASHAReportFinalSLP2024.qmd
├── SLP2024- Preliminary Report.qmd
├── SLP School.qmd
├── docs/
│   ├── project_overview.md
│   ├── methods_summary.md
│   ├── repository_structure.md
│   └── limitations_and_qa.md
├── analysis/
│   └── README.md
└── outputs/
    └── README.md
```

## Main Files

### Analysis Files

- `ASHAReportFinalSLP2024.qmd`: Final/report-style Quarto workflow for the SLP survey methodology analysis.
- `SLP2024- Preliminary Report.qmd`: Preliminary report with postcard intervention effects, survey mode analysis, logistic regression interpretation, and recommendations.
- `SLP School.qmd`: Additional SLP Schools analysis file.

### Documentation

- `docs/project_overview.md`: Research motivation, questions, data context, and outputs.
- `docs/methods_summary.md`: Summary of data preparation, postcard analysis, bootstrap inference, mode comparisons, and inferential tests.
- `docs/limitations_and_qa.md`: Interpretation limits, treatment-by-indication caution, confidentiality, and QA checklist.
- `docs/repository_structure.md`: Explanation of repository layout.

### Analysis and Outputs Directories

- `analysis/README.md`: Explains the current analysis files and suggested future cleaned structure.
- `outputs/README.md`: Documents the expected output categories, including response-rate tables, postcard estimates, mode-comparison figures, and logistic regression summaries.

## Skills Demonstrated

- Survey methodology
- Response-rate analysis
- Nonresponse evaluation
- Mode effects
- Postcard/follow-up experiment analysis
- Policy estimands
- Bootstrap inference
- Logistic regression
- Chi-square tests
- Subgroup analysis
- R/Quarto reproducible reporting
- Stakeholder-facing recommendations

## Reproducibility

1. Clone the repository:

```bash
git clone https://github.com/Sagnik-Chakravarty/ASHA.git
```

2. Open the Quarto files in RStudio or another Quarto-compatible environment.

3. Install required packages, as needed:

```r
install.packages(c("tidyverse", "survey", "broom", "ggplot2", "kableExtra"))
```

4. Render the report files to inspect the analysis and recommendations.

## Confidentiality Note

This repository documents analysis workflows and methods. Respondent-level survey files should not be publicly released unless de-identified and approved for sharing.

## Authors

- **Sagnik Chakravarty**  
  University of Maryland, Joint Program in Survey Methodology  
  Portfolio: https://sagnik-chakravarty.github.io/

- **Ruisi Ma**  
  University of Michigan

- **Yuchen Ding**  
  University of Michigan

- **Feiran Ge**  
  University of Michigan
