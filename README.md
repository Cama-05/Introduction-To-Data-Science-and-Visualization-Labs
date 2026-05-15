# 📊 Introduction to Data Science and Visualization — Labs

> **Course:** Introduction to Data Science and Visualization
> **Academic Year:** 2025/2026
> **Institution:** Politecnico di Torino
> **Author:** Matteo Camastra

---

## 📖 Overview

This repository contains all laboratory sessions for the *Introduction to Data Science and Visualization* course (A.Y. 2025/2026) at Politecnico di Torino.

The labs follow a structured learning path: starting from spreadsheet-based descriptive statistics, progressing through Python data manipulation and wrangling, advancing into visualization using the grammar of graphics paradigm, and culminating in numerical computing and critical awareness of data science pitfalls. Each lab is self-contained in its own folder with a dedicated notebook (or Excel files), dataset, and `README.md`.

---

## 🗂️ Repository Structure

```
.
├── dsv-lab-1/       # Descriptive Statistics with Excel
├── dsv-lab-2/       # Introduction to Jupyter & Pandas
├── dsv-lab-3/       # Data Wrangling with Pandas
├── dsv-lab-3b/      # Dataset Querying & Basic Plots
├── dsv-lab-4/       # Grammar of Graphics with Plotnine
├── dsv-lab-5/       # Numerical Computing with NumPy
├── dsv-lab-6/       # Advanced Visualization & Inferential Statistics
├── dsv-lab-7/       # Fraud Detection Pipeline
└── requirements.txt # Global Python dependencies
```

---

## 🧪 Labs at a Glance

| # | Folder | Name | Description | Key Libraries / Tools |
|---|--------|------|-------------|-----------------------|
| 1 | [`dsv-lab-1`](dsv-lab-1/) | **Descriptive Statistics in Excel** | Summary statistics (mean, median, IQR, MAD, range), frequency tables with pivot and `COUNTIF`, and basic chart types. Datasets: Serie A top scorers (2025/26) and Italian parliamentary declared assets (OpenPolis). | Microsoft Excel |
| 2 | [`dsv-lab-2`](dsv-lab-2/) | **Intro to Jupyter & Pandas** | First contact with Jupyter Notebooks and Python. Simple dataset loading, inspection, and manipulation. | `pandas` |
| 3 | [`dsv-lab-3`](dsv-lab-3/) | **Data Wrangling** | Wrangling of ISTAT Italian employment data (Jan 2026). Cleaning, reshaping, and transforming multi-sheet Excel data into tidy DataFrames. | `pandas`, `openpyxl` |
| 3b | [`dsv-lab-3b`](dsv-lab-3b/) | **Dataset Querying & Basic Plots** | Querying and filtering the ISTAT employment dataset. Introduction to basic line and bar plots. | `pandas`, `matplotlib` |
| 4 | [`dsv-lab-4`](dsv-lab-4/) | **Grammar of Graphics — Basics** | Introduction to the grammar of graphics paradigm using `plotnine` (ggplot2-style). Exploratory visual analysis of the Netflix titles dataset (8,800+ entries). | `pandas`, `plotnine` |
| 5 | [`dsv-lab-5`](dsv-lab-5/) | **Numerical Computing with NumPy** | Fundamentals of NumPy: array creation, indexing, broadcasting, and numerical operations applied to synthetic datasets. | `numpy` |
| 6 | [`dsv-lab-6`](dsv-lab-6/) | **Advanced Visualization & Inferential Statistics** | Customized and polished `plotnine` charts; introduction to inferential statistics (hypothesis testing, distributions) using `scipy`. Dataset: Netflix titles. | `pandas`, `plotnine`, `numpy`, `scipy` |
| 7 | [`dsv-lab-7`](dsv-lab-7/) | **Fraud Detection Pipeline** | End-to-end data science pipeline for binary fraud classification on a synthetic bank transactions dataset. Covers feature engineering, model selection, and evaluation — with a strong focus on avoiding common pitfalls: data leakage, train/test contamination, imbalanced class metrics, cross-validation strategy, and decision threshold tuning. | `pandas`, `numpy`, `scikit-learn`, `matplotlib` |

---

## 🛠️ Setup & Requirements

### Prerequisites

- Python 3.11+
- JupyterLab or VS Code with the Jupyter extension

### Install dependencies

Each lab manages its own dependencies independently. Navigate into the lab folder and install from its local `requirements.txt`:

```bash
cd dsv-lab-X

# (Recommended) Create a virtual environment
python -m venv .venv
source .venv/bin/activate        # macOS / Linux
.venv\Scripts\activate           # Windows

# Install lab-specific dependencies
pip install -r requirements.txt
```

> **Note:** Labs 5, 6, and 7 also support [uv](https://docs.astral.sh/uv/) as an optional fast package manager — each of those folders includes a `pyproject.toml` and `uv.lock` file for reproducible installs.

---

## 📦 Core Libraries

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, manipulation, and wrangling |
| `matplotlib` | Low-level 2D plotting |
| `plotnine` | Grammar of graphics visualization (ggplot2-style) |
| `numpy` | Numerical arrays and mathematical operations |
| `scipy` | Inferential statistics and scientific computing |
| `scikit-learn` | Machine learning models and evaluation metrics |
| `openpyxl` | Reading and writing Excel (`.xlsx`) files |
| `jupyterlab` | Interactive notebook environment |

---

## 📚 Datasets Used

| Dataset | Source | Lab(s) |
|---------|--------|--------|
| Serie A Top Scorers 2025/26 (Matchday 25) | [Corriere della Sera](https://www.corriere.it/sport/calcio/serie-a/marcatori/) | Lab 1 |
| Italian Parliamentary Declared Assets (2014) | [OpenPolis](http://www.openpolis.it) | Lab 1 |
| Italian Employment Data — ISTAT Jan 2026 | [ISTAT](https://www.istat.it/comunicato-stampa/occupati-e-disoccupati-dati-provvisori-gennaio-2026) | Lab 3, 3b |
| Netflix Titles (8,800+ movies & TV shows) | [Kaggle / TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-04-20/readme.md) | Lab 4, 6 |
| Synthetic Bank Fraud Transactions | Synthetic (course-provided) | Lab 7 |

---

## 📄 License

This repository is for educational purposes only. All datasets belong to their respective owners and are used solely for academic learning. No commercial use intended.
