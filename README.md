# Optimization Models and Methods - Group Project

## Project Overview

This is a group project for the Optimization Models and Methods course, focusing on linear programming and integer programming optimization problems.

## Team Members

- Member 1: [Name]
- Member 2: [Name]
- Member 3: [Name]
- Member 4: [Name]

## Project Structure

```
Opt_Group/
├── README.md                    # Project documentation
├── requirements.txt             # Python dependencies
├── .gitignore                   # Git ignore configuration
├── data/                        # Data directory
│   ├── raw/                     # Raw data
│   └── processed/               # Processed data
├── src/                         # Source code
│   ├── models/                  # Optimization model definitions
│   ├── solvers/                 # Solver implementations
│   └── utils/                   # Utility functions
├── notebooks/                   # Jupyter notebooks for exploration and analysis
├── results/                     # Experimental results
│   ├── figures/                 # Figures and plots
│   └── tables/                  # Data tables
├── report/                      # LaTeX project report
│   ├── main.tex                 # Main document
│   ├── sections/                # Report sections
│   ├── figures/                 # Figures for report
│   └── references.bib           # Bibliography
└── tests/                       # Unit tests
```

## Environment Setup

### 1. Clone Repository

```bash
git clone https://github.com/bayerworld233-svg/Opt_Group.git
cd Opt_Group
```

### 2. Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. (Optional) Install Commercial Solvers

If you need to use Gurobi or CPLEX:
- Obtain academic license
- Install the corresponding Python package
- Configure license file

## Usage

### Run Optimization Model

```bash
python src/models/your_model.py
```

### Run Jupyter Notebook

```bash
jupyter notebook notebooks/
```

### Compile LaTeX Report

```bash
cd report
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Project Timeline

- [ ] Problem definition and literature review
- [ ] Data collection and preprocessing
- [ ] Model design and implementation
- [ ] Algorithm solving and results analysis
- [ ] Report writing
- [ ] Final presentation preparation

## Contributing

1. Create a new feature branch from `main`
2. Develop on the new branch
3. Ensure code runs properly before committing
4. Create Pull Request and request review

## License

This project is for academic purposes only.

## Contact

For questions, please contact: [your-email@example.com]
