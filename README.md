# Practical-programming-in-chemistry-semester-project-
# Practical Programming in Chemistry — Semester Project

> Semester project for **CH-200 / Practical Programming in Chemistry** at EPFL.

<!-- Optional badges — uncomment and adapt once relevant -->
<!--
![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
-->

## About

This repository contains our semester project for the EPFL course **CH-200: Practical Programming in Chemistry**. The project applies Python programming and modern software-development practices (version control, modular code, testing, documentation) to a chemistry-related problem.

> **TODO:** Replace this paragraph with a 2–4 sentence description of *what the project actually does* — the chemistry/scientific problem you tackle, the methods or models you implement, and what the user gets out of running it.

## Features

- *(Replace these placeholders with the actual capabilities of your project)*
- Loads and processes chemical/experimental data from standard formats (`.csv`, `.xlsx`, …)
- Performs the core analysis / computation specific to the project
- Generates plots and summary tables of the results
- Provides a reproducible workflow via Jupyter notebooks and/or a Python module

## Installation

### Prerequisites

- Python ≥ 3.10
- `git`
- (Optional but recommended) [Conda](https://docs.conda.io/) or `venv` for environment management

### Clone the repository

```bash
git clone https://github.com/BogdanFilipchuk/Practical-programming-in-chemistry-semester-project-.git
cd Practical-programming-in-chemistry-semester-project-
```

### Set up the environment

Using `venv`:

```bash
python -m venv venv
source venv/bin/activate          # macOS / Linux
source venv/Scripts/activate      # Windows (Git Bash)
pip install -r requirements.txt
```

Or using Conda:

```bash
conda create -n ppchem python=3.10
conda activate ppchem
pip install -r requirements.txt
```

## Usage

### Running the main script

```bash
python src/main.py --input data/sample.csv --output results/
```

### Using the Jupyter notebooks

```bash
jupyter notebook notebooks/
```

Open the notebook of interest (e.g. `notebooks/analysis.ipynb`) and run the cells in order.

### Example

```python
from ppchem import analyze

results = analyze("data/sample.csv")
results.summary()
results.plot()
```

> **TODO:** Replace the example above with a real, runnable snippet from your project, and add a representative output (numbers, a screenshot of a plot, etc.).

## Project Structure

```
.
├── data/              # Input datasets (raw and processed)
├── notebooks/         # Jupyter notebooks for exploration and analysis
├── src/               # Source code (Python modules)
│   └── ppchem/
├── tests/             # Unit tests
├── results/           # Generated figures and output files
├── requirements.txt   # Python dependencies
├── LICENSE
└── README.md
```

## Testing

To run the unit tests:

```bash
pytest tests/
```

## Contributors

This project was developed as part of the CH-200 course at EPFL by:

| Name | Email |
|------|-------|
| Maximus Vandenbogaard | [maximus.vandenbogaard@epfl.ch](mailto:maximus.vandenbogaard@epfl.ch) |
| Bogdan Filipchuk      | [bogdan.filipchuk@epfl.ch](mailto:bogdan.filipchuk@epfl.ch) |
| Tuna Karasu           | [tuna.karasu@epfl.ch](mailto:tuna.karasu@epfl.ch) |
| Andrey Babenko        | [andrey.babenko@epfl.ch](mailto:andrey.babenko@epfl.ch) |

## License

This project is released under the MIT License — see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Developed for **CH-200 — Practical Programming in Chemistry** at [EPFL](https://www.epfl.ch/), Section de Chimie et Génie Chimique.
- Thanks to the course staff for guidance and feedback.
- Built with the open-source Python scientific stack: NumPy, pandas, Matplotlib, SciPy, and Jupyter.
- AI usage - LLM models such as ChatGPT and Claude were used for drafting, debugging and implementing parts of the code. The final version of the project is fully concieved by the authors. 
