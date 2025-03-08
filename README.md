# UrbanBikeFlow

A Python project structured using **Cookiecutter Data Science**, with **UV** for dependency management and **GitHub** for version control.

## 📂 Project Structure

This project follows the [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science) template:

```
├── README.md          # Project overview and instructions
├── data/             # Data storage (not tracked by Git)
│   ├── external/     # Data from external sources
│   ├── interim/      # Intermediate data transformations
│   ├── raw/          # Original data
│   └── processed/    # Final processed data
├── docs/             # Documentation
├── models/           # Trained models and outputs
├── notebooks/        # Jupyter notebooks
├── reports/          # Generated analysis and figures
│   └── figures/      # Visual outputs and plots
├── src/              # Source code
│   ├── __init__.py   # Package initialization
│   └── your_module/  # Main package
└── pyproject.toml    # Project metadata and dependencies
```

## 🚀 Getting Started

### Prerequisites

Ensure **UV** is installed:

```bash
pip install uv
```

### Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/cyclingMoritz/UrbanBikeFlow.git
cd UrbanBikeFlow
```

2. Create and activate a virtual environment:

```bash
uv venv
source .venv/bin/activate   # Linux/macOS
.venv\Scripts\activate      # Windows
```

3. Install dependencies from `pyproject.toml`:

```bash
uv pip install
```

4. Run the main script:

```bash
python src/main.py
```

## 📦 Managing Dependencies

Add new packages using UV:

```bash
uv pip install package-name
```

Update the `pyproject.toml` by syncing dependencies:

```bash
uv pip freeze > pyproject.toml
```

## 📊 Project Workflow

1. Add your code under `src/`.
2. Use `notebooks/` for experiments.
3. Organize data into `data/external`, `data/interim`, `data/raw`, and `data/processed`.
4. Store models in `models/`.
5. Save reports and figures in `reports/` and `reports/figures/`.

## 🔗 Contributing

1. Fork the repository and create a feature branch:

```bash
git checkout -b feature/your-feature
```

2. Make changes and commit:

```bash
git add .
git commit -m "Add new feature"
```

3. Push and open a pull request:

```bash
git push origin feature/your-feature
```

## 📜 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

