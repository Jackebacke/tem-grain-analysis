# tem-grain-analysis

AI-assisted grain tracking and quantitative analysis of in situ TEM videos.

## Project goal

The project aims to automate or semi-automate the identification and tracking
of individual grains in time-resolved TEM videos. The planned analysis covers
grain size, shape, position, displacement, growth, shrinkage, merging,
disappearance, and population statistics.

## Repository layout

```text
.
├── configs/                # YAML configuration for each pipeline stage
├── docs/                   # Project documentation and requirements
├── notebooks/              # Exploratory and evaluation notebooks
├── outputs/                # Generated analysis results
├── scripts/                # Reusable pipeline and result-inspection scripts
├── src/graintrack/
│   ├── analysis/           # Grain tracking and population analysis
│   ├── human_correction/   # Manual correction workflow
│   ├── io/                 # Video and data input/output
│   ├── measurements/       # Grain property calculations
│   ├── preprocessing/      # Image preparation
│   ├── segmentation/       # Grain segmentation methods
│   └── visualization/      # Diagnostic and result visualizations
├── pyproject.toml
└── README.md
```

## Setup

Create an environment and install the project with development tools:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -e ".[dev]"
```

Run the tests and inspect the command-line scaffold:

```bash
pytest
graintrack
```
