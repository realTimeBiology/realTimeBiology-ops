# realTimeBiology-ops

Operations repository for realTimeBiology.

## Overview

This repository contains code, analysis, pipelines, and technical infrastructure for the venture. It complements the Google Drive structure by providing version control for all technical assets.

## Repository Structure

```
realTimeBiology-ops/
├── analysis/           # Analysis scripts and Jupyter notebooks
├── pipelines/          # Data processing and computational pipelines
├── infrastructure/     # Infrastructure as code (Docker, Terraform, etc.)
├── tools/              # Internal utilities and automation scripts
├── docs/               # Technical documentation
└── .github/            # GitHub workflows and templates
```

## Getting Started

### Prerequisites

- Python 3.8+ (for analysis scripts)
- Docker (optional, for containerized workflows)
- Access to the venture's Google Drive (link below)

### Installation

```bash
# Clone the repository
git clone https://github.com/realTimeBiology/realTimeBiology-ops.git
cd realTimeBiology-ops

# Set up Python environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies (if requirements.txt exists)
pip install -r requirements.txt
```

## Directory Details

### analysis/
Analysis scripts, Jupyter notebooks, and exploratory data analysis. Keep analysis reproducible and document data sources.

**Organization:**
- Use descriptive names with dates: `2024-03-15_experiment_analysis.ipynb`
- Include data source paths in notebook headers
- Export key results to processed data in Google Drive

### pipelines/
Production-grade data processing and computational pipelines.

**Organization:**
- One directory per pipeline: `pipelines/target_design/`, `pipelines/screening_analysis/`
- Include README with pipeline description, inputs, outputs
- Use configuration files for parameters
- Add tests for critical functions

### infrastructure/
Infrastructure as code, deployment configs, and environment setup.

**Examples:**
- Docker containers for computational tools
- Cloud infrastructure (Terraform/CloudFormation)
- Database schemas and migrations
- Environment configuration files

### tools/
Internal utilities, automation scripts, and helper tools.

**Examples:**
- Data validation scripts
- Report generation tools
- Workflow automation
- Integration scripts (Google Drive sync, etc.)

### docs/
Technical documentation, API references, and guides.

**Include:**
- Architecture decisions and rationale
- API documentation for internal tools
- Setup guides for complex systems
- Troubleshooting guides

## Links

- **Google Drive Structure**: [Link to shared drive]
- **Organization**: realTimeBiology
- **Main Template Repository**: https://github.com/Arielbs/venture-ops-template

## Development Guidelines

### Code Style
- Follow PEP 8 for Python code
- Use type hints where appropriate
- Document functions with docstrings
- Keep functions small and focused

### Git Workflow
- Use feature branches: `feature/description`
- Write clear commit messages
- Review code before merging to main
- Tag releases for important milestones

### Data Management
- **Never commit large data files** - use Git LFS or store in Google Drive
- Keep raw data in Google Drive `science/data/raw_data/`
- Store processed results in Google Drive `science/data/processed_data/`
- Reference data locations in code/notebooks

### Testing
- Add tests for critical functions
- Use pytest for Python testing
- Run tests in CI/CD before merging

## Common Tasks

### Running Analysis
```bash
cd analysis
jupyter notebook  # Opens Jupyter in browser
```

### Running a Pipeline
```bash
cd pipelines/your_pipeline
python run_pipeline.py --config config.yaml
```

### Building Docker Images
```bash
cd infrastructure/docker
docker build -t realTimeBiology/tool-name:latest .
```

## Contributing

1. Create a feature branch
2. Make your changes
3. Add tests if applicable
4. Submit a pull request
5. Get review from team member
6. Merge after approval

## Support

For questions or issues:
- Check the docs/ directory
- Review existing issues in GitHub
- Ask in the team Slack channel
- Contact the tech lead

## License

[Add your license here]
