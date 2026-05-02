# Methods Summary

## 1. Data Preparation

The project uses respondent files and full sample-frame files. The analysis workflow compares respondent records against the full sample to identify respondents, nonrespondents, mode assignments, and subgroup characteristics.

Core preparation steps include:

- importing respondent and sample-frame files,
- cleaning and harmonizing IDs,
- identifying eligible sampled units,
- constructing response indicators,
- merging respondent and full sample records,
- creating subgroup variables for age, employment, facility type, and region.

## 2. Postcard Reminder Analysis

The postcard analysis evaluates the effect of follow-up reminders on survey response. Because postcard receipt depends on nonresponse status at earlier stages, the project avoids naive comparisons of zero-, one-, and two-postcard groups.

The analysis uses a sequential response framework with conditional response-rate components:

- baseline response before postcard intervention,
- response among nonrespondents assigned to no postcard,
- response among nonrespondents assigned to the first postcard,
- response after the first postcard among those assigned to only one postcard,
- response after the first postcard among those assigned to a second postcard.

This supports policy estimands for response rates under no postcard, one postcard, and two postcard regimes.

## 3. Bootstrap Inference

Bootstrap resampling is used to estimate uncertainty around postcard effect estimates. The workflow repeatedly resamples records and recalculates response-rate quantities to produce uncertainty estimates for follow-up effects.

## 4. Short-Term Follow-Up Effects

The project examines whether response rates increase immediately after follow-up mailings. This uses response timing and pre/post comparison windows around postcard dates.

The design is related to a difference-in-differences style comparison of response activity before and after reminder contact.

## 5. Survey Mode Analysis

The mode analysis compares postal mail and web/SurveyMonkey administration.

Core outputs include:

- overall response-rate comparisons,
- subgroup response-rate tables,
- mode gaps by age, employment status, facility type, and region,
- composition checks to assess whether mode changes respondent profile.

## 6. Inferential Tests

The project uses several inferential tools:

- Pearson chi-square tests for mode-response associations,
- logistic regression models for response propensity,
- interaction models for subgroup-specific mode effects,
- likelihood ratio tests for comparing nested models.

## 7. Interpretation Framework

The project is interpreted through survey methodology concepts including:

- nonresponse error,
- mode effects,
- treatment by indication,
- policy estimands,
- respondent burden,
- Total Survey Error.

The goal is to convert empirical response patterns into practical survey-design recommendations.
