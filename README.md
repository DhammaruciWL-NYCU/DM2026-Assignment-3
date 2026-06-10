# Data Mining (DM2026) - Assignment 3
**By:** Dhammaruci Wiradhika Lungadhi (314540050)

## Project Overview
This repository contains the implementation for Assignment 3 of the Data Mining course. The primary objective is to process the provided dataset and train an ensemble of LightGBM classifiers. The methodology utilizes seed averaging to stabilize model predictions, ultimately generating a final output file (`submission_seed_averaging_06.csv`) for Kaggle evaluation.

## Repository Structure
    DM2026-Assignment-3/
    ├── .gitignore
    ├── README.md
    ├── Data_Mining_Assignment_3_Notebook.ipynb
    └── requirements.txt (Optional but recommended)

## Prerequisites and Dependencies
Execution of this notebook requires Python 3.8 or higher. The following Python libraries are strictly required:
* `pandas`
* `numpy`
* `scikit-learn`
* `lightgbm`
* `kagglehub`
* `jupyter`

## Setup and Execution Instructions

### Step 1: Clone the Repository
Clone this repository to your local machine:
    git clone https://github.com/DhammaruciWL-NYCU/DM2026-Assignment-3.git
    cd DM2026-Assignment-3

### Step 2: Environment Configuration
Isolate the dependencies by creating and activating a virtual environment.

**Linux/macOS:**
    python -m venv venv
    source venv/bin/activate
    pip install pandas numpy scikit-learn lightgbm kagglehub jupyter

**Windows:**
    python -m venv venv
    venv\Scripts\activate
    pip install pandas numpy scikit-learn lightgbm kagglehub jupyter

### Step 3: Kaggle API Authentication
The notebook uses `kagglehub` to download the dataset dynamically. You must authenticate with the Kaggle API.
1. Log into Kaggle.
2. Go to your Account settings and select "Create New API Token". This downloads a `kaggle.json` file.
3. Place this file in the appropriate directory for your OS:
   * **Linux/macOS:** `~/.kaggle/kaggle.json`
   * **Windows:** `C:\Users\<Your-Username>\.kaggle\kaggle.json`
4. Secure the credentials (Linux/macOS only): `chmod 600 ~/.kaggle/kaggle.json`

### Step 4: Run the Notebook
Launch the Jupyter Notebook server:
    jupyter notebook

1. Open `Data_Mining_Assignment_3_Notebook.ipynb`.
2. Ensure the kernel is set to the virtual environment you created.
3. Select **"Restart & Run All"** from the Kernel menu to execute the pipeline from start to finish.
4. Upon successful execution, the script will output the probability predictions into a file named `submission_seed_averaging_06.csv` in the root directory.
