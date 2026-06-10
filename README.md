# Data Mining (DM2026) - Assignment 3

**By:** Dhammaruci Wiradhika Lungadhi  
**Student ID:** 314540050

## Project Overview

This repository contains my submission for Assignment 3 of the Data Mining course.

## Original Kaggle Notebook

This project was originally developed and executed in Kaggle Notebook.

Kaggle Notebook:
https://www.kaggle.com/code/dhammaruciwl/dm2026-assignment-3-notebook

The GitHub repository is the official submission version and contains only necessary source code found in the report. The Kaggle notebook is provided as a reference environment in case of local dependency or platform-specific issues. The original source code that serves as the testing ground are available in another notebook which contains a more detailed results but harder to go through.

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
   /n(note 1: The notebook still preserves the output produced on the initial runs, if you wish to re-test it yourself please proceed to the next step.)
   /n(note 2: it might take too long to complete the whole run as inside the notebook contains multiple cells with different models training, otherwise only run cell 1,3 and your designated model cell.)
6. Run all cells from top to bottom:
   - Kernel → Restart & Run All

## Expected Output

The notebook should generate the final submission file in the repository root:

```text
submission_seed_averaging.csv
```

## Notes

- Do not commit Kaggle credentials.
- Do not commit large raw dataset files unless explicitly required.
- If you add or remove imports in the notebook, update `requirements.txt`.
- Before submission, restart the kernel and run all cells once to confirm the notebook works cleanly from start to finish.
