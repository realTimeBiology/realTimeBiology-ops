# Pipelines

Production-grade data processing and computational pipelines.

## Organization

Each pipeline should have its own directory with:
- `README.md` - Description, inputs, outputs, usage
- `config.yaml` - Configuration parameters
- `run_pipeline.py` - Main entry point
- `tests/` - Unit tests for pipeline components

## Example Pipeline Structure

```
pipelines/
├── protein_design/
│   ├── README.md
│   ├── config.yaml
│   ├── run_pipeline.py
│   ├── modules/
│   │   ├── structure_prep.py
│   │   ├── design.py
│   │   └── validation.py
│   └── tests/
│       └── test_design.py
└── screening_analysis/
    ├── README.md
    ├── config.yaml
    └── run_pipeline.py
```

## Best Practices

1. **Configuration**: Use config files for parameters, never hardcode
2. **Logging**: Log progress and errors clearly
3. **Testing**: Test critical functions
4. **Documentation**: Document inputs, outputs, and expected runtime
5. **Error Handling**: Gracefully handle failures and provide clear error messages
