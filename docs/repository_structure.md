# Repository Structure

This repository preserves the original ASHA survey methodology analysis files while adding professional documentation for reviewer and portfolio use.

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

## Main Analysis Files

- `ASHAReportFinalSLP2024.qmd`: Final/report-style Quarto analysis for the SLP survey methodology project.
- `SLP2024- Preliminary Report.qmd`: Preliminary report with methods, postcard intervention estimates, mode effects, subgroup analysis, logistic regression interpretation, and recommendations.
- `SLP School.qmd`: Additional SLP Schools survey analysis file.

## Documentation

- `docs/project_overview.md`: Research motivation, questions, data context, and outputs.
- `docs/methods_summary.md`: Data preparation, postcard analysis, bootstrap inference, mode analysis, and inferential tests.
- `docs/repository_structure.md`: This file.
- `docs/limitations_and_qa.md`: Notes on interpretation limits, data-quality checks, and confidentiality.

## Suggested Future Cleanup

A production-level version could reorganize files into:

```text
analysis/
  01_data_preparation.qmd
  02_postcard_experiment.qmd
  03_mode_effects.qmd
  04_final_report.qmd
outputs/
  tables/
  figures/
docs/
```

The current repository keeps the original file names and paths to avoid breaking existing project links.
