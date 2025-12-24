# Tools

Internal utilities, automation scripts, and helper tools.

## Organization

Group tools by function:
- **data/** - Data validation, cleaning, transformation
- **automation/** - Workflow automation, scheduled tasks
- **reporting/** - Report generation, metrics dashboards
- **integration/** - Scripts for integrating systems (Drive, databases, etc.)

## Best Practices

1. **CLI First**: Make tools runnable from command line
2. **Help Text**: Include clear usage instructions (--help flag)
3. **Configuration**: Use config files or environment variables
4. **Logging**: Log operations for debugging
5. **Testing**: Test edge cases and error conditions

## Example Structure

```
tools/
├── data/
│   ├── validate_experimental_data.py
│   └── transform_plate_reader_output.py
├── automation/
│   ├── sync_drive_to_s3.py
│   └── generate_weekly_report.py
└── reporting/
    ├── dashboard_generator.py
    └── metrics_calculator.py
```
