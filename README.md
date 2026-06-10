# Data Mining (DM2026) - Assignment 3

**Author:** Dhammaruci Wiradhika Lungadhi  
**Student ID:** 314540050

## Project Overview

This repository contains my submission for Assignment 3 of the Data Mining course.

The notebook:
- loads and preprocesses the dataset
- trains machine learning models
- performs seed averaging
- generates the final Kaggle submission file

## Repository Contents

```text
DM2026-Assignment-3/
├── .gitignore
├── README.md
├── requirements.txt
└── Data_Mining_Assignment_3_Notebook.ipynb
```

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Kaggle account
- Kaggle API token (`kaggle.json`) if dataset access requires authentication

## Installation

Create a virtual environment and install the dependencies.

### macOS / Linux

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Windows

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Kaggle Setup

If the notebook uses Kaggle API access:

1. Log in to Kaggle.
2. Go to your account settings.
3. Create a new API token.
4. Download `kaggle.json`.
5. Place it in the correct location.

### macOS / Linux

```bash
mkdir -p ~/.kaggle
mv kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

### Windows

Place `kaggle.json` in:

```text
C:\Users\<Your-Username>\.kaggle\kaggle.json
```

## How to Run

1. Open a terminal in the repository folder.
2. Activate the virtual environment.
3. Start Jupyter:

```bash
jupyter notebook
```

4. Open `Data_Mining_Assignment_3_Notebook.ipynb`.
5. Run all cells from top to bottom:
   - Kernel → Restart & Run All

## Expected Output

The notebook should generate the final submission file in the repository root:

```text
submission_seed_averaging_06.csv
```

## Notes

- Do not commit Kaggle credentials.
- Do not commit large raw dataset files unless explicitly required.
- If you add or remove imports in the notebook, update `requirements.txt`.
- Before submission, restart the kernel and run all cells once to confirm the notebook works cleanly from start to finish.
