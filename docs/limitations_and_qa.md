# Limitations and Quality-Assurance Notes

## Interpretation Limits

This project evaluates survey design decisions using available ASHA survey files. The results should be interpreted as evidence about response behavior under the specific survey designs, populations, and fielding conditions studied.

## Treatment by Indication

The postcard reminder analysis requires careful interpretation because respondents become eligible for later postcard contacts only if they have not responded earlier. Naively comparing zero-, one-, and two-postcard groups can be misleading. The project therefore emphasizes conditional response rates and policy estimands rather than simple post-hoc group comparisons.

## Mode Comparison Limits

Postal mail and web response differences may reflect both mode effects and subgroup response tendencies. The analysis uses subgroup comparisons and regression models to evaluate these patterns, but mode comparisons should still be interpreted in relation to the sampling frame, contact protocol, and survey topic.

## Data Confidentiality

Respondent-level survey files should not be publicly released unless de-identified and approved for sharing. This repository is intended to document analysis workflows, methods, and outputs, not to expose confidential respondent data.

## Recommended QA Checks

Before finalizing any survey analysis, the following checks should be performed:

| QA Area | Check |
|---|---|
| ID matching | Confirm respondent IDs merge correctly with the full sample frame |
| Eligibility | Verify exclusion rules for ineligible cases, bounced contacts, or invalid records |
| Response indicator | Confirm respondent/nonrespondent coding across modes |
| Mode assignment | Validate mail vs. web/SurveyMonkey assignment |
| Postcard timing | Confirm dates of first and second postcards and response timing |
| Subgroup variables | Check age, employment, region, and facility coding |
| Missingness | Identify missing values in key subgroup variables |
| Regression inputs | Confirm model sample size and complete-case rules |
| Output tables | Check denominators for all response-rate calculations |
| Confidentiality | Remove direct identifiers from public outputs |

## Recommended Reporting Practices

- Report denominators clearly for every response-rate estimate.
- Distinguish descriptive comparisons from causal/policy estimands.
- Avoid claiming that later postcard groups are directly comparable without conditioning on nonresponse status.
- Present subgroup mode effects with both rates and differences where possible.
- Use figures and tables to support stakeholder recommendations.
