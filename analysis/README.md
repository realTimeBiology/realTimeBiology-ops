# Analysis

This directory contains analysis scripts and Jupyter notebooks.

## Organization

- Use descriptive names with dates: `2024-03-15_experiment_analysis.ipynb`
- Group related analyses in subdirectories
- Document data sources at the top of each notebook
- Export key results to Google Drive's `science/data/processed_data/`

## Best Practices

1. **Reproducibility**: Include all dependencies in requirements.txt
2. **Documentation**: Add markdown cells explaining your analysis
3. **Data References**: Use relative paths or environment variables for data locations
4. **Version Control**: Commit notebooks with cleared outputs to avoid large diffs

## Example Structure

```
analysis/
├── exploratory/
│   └── 2024-03-15_initial_screening_eda.ipynb
├── publications/
│   └── 2024-05-01_paper_figure_generation.ipynb
└── reports/
    └── 2024-04-01_monthly_metrics.ipynb
```
