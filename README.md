# MLX Is All You Need

A comprehensive repository for developing, training, and deploying ML models with MLX - Apple's open-source machine learning framework optimized for Apple Silicon.

## About

MLX is Apple's machine learning framework designed specifically for Apple Silicon, offering exceptional performance by leveraging the full power of the unified memory architecture and the Neural Engine in Apple's M-series chips. This repository provides templates, tools, and best practices for building machine learning projects with MLX.

## Features

- 🚀 **Apple Silicon Optimization** - Leverage the full power of M-series chips
- ⚡ **High-Performance ML** - Faster training and inference with MLX
- 📊 **Experiment Tracking** - Integrated MLflow for tracking experiments
- 🧩 **Modular Structure** - Well-organized project templates for all ML workflow stages
- 🛠️ **Ready-to-Use Tools** - Utilities for data processing, model training, and evaluation

## Project Structure

```
MLXisAllYouNeed/
├── src/                    # Source code
│   ├── data/               # Data processing modules
│   ├── models/             # Model definitions
│   ├── training/           # Training logic
│   ├── inference/          # Inference code
│   └── evaluation/         # Evaluation utilities
├── data/                   # Data storage (excluded from git)
│   ├── raw/                # Original data
│   └── processed/          # Processed data
├── models/                 # Model storage
│   ├── pretrained/         # Downloaded pre-trained models
│   ├── mlx/                # MLX-converted models
│   └── deployed/           # Production-ready models
├── docs/                   # Documentation
│   └── ON_MLOpsBestPractice.md  # MLOps best practices guide
├── scripts/                # Utility scripts
│   └── setup/              # Setup scripts
│       └── quickstart.sh   # Project initialization script
└── templates/              # Template modules
    ├── data/               # Data processing templates
    ├── models/             # Model templates
    ├── training/           # Training templates
    ├── inference/          # Inference templates
    └── evaluation/         # Evaluation templates
```

## Getting Started

### Prerequisites

- macOS running on Apple Silicon (M1/M2/M3 series)
- Python 3.9+
- Git

### Quick Setup

The repository includes a comprehensive setup script that creates a fully configured MLX project:

```bash
# Clone the repository
git clone https://github.com/octonova-ai/mlxisallyouneed.git
cd mlxisallyouneed

# Run the quickstart script
bash scripts/setup/quickstart.sh your_project_name
```

The quickstart script:
- Creates a structured ML project
- Sets up a Python virtual environment
- Installs MLX and dependencies
- Configures MLflow for experiment tracking
- Adds templates for data, models, training, and inference
- Initializes Git repository with appropriate .gitignore

### Manual Setup

If you prefer to set up manually:

```bash
# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate

# Install core dependencies
pip install mlx numpy pandas scikit-learn matplotlib

# Install experiment tracking
pip install mlflow

# Install additional utilities
pip install tqdm safetensors
```

## Documentation

- `docs/ON_MLOpsBestPractice.md` - Comprehensive guide to MLOps best practices with MLX
- Template files include detailed documentation and examples

## MLX Model Workflow

1. **Data Processing**: Load and prepare datasets for training
2. **Model Definition**: Create or load MLX model architecture
3. **Training**: Train models with MLX optimization
4. **Evaluation**: Assess model performance
5. **Deployment**: Deploy models for inference

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [MLX Team at Apple](https://github.com/ml-explore/mlx)
- OctoNova AI for providing templates and best practices 