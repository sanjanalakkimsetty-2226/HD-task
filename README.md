# HD Task — Heart Attack Prediction

This repository contains the reproducible implementation for the HD machine learning task based on the paper:

**M. Bhagat, A. Sharma, and P. Agarwal, “An efficient stacking-based ensemble technique for early heart attack prediction,” Multimedia Tools and Applications, 2025.**

## Repository contents

- `11.1 hd task.ipynb` — main Jupyter notebook containing the reproduction study and proposed improved method.
- `heart.csv` — heart disease dataset used by the notebook.
- `requirements.txt` — Python package requirements.
- `README.md` — installation and execution instructions.

## Dataset

The notebook uses `heart.csv`, which is included in this repository so the project can run from a fresh clone without any additional manual download step.

Expected dataset columns:

`age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal, target`

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/sanjanalakkimsetty-2226/HD-task.git
cd HD-task
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**macOS / Linux**

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

If XGBoost is not installed correctly, run:

```bash
pip install xgboost
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

`HD_Task_Heart_Attack_FINAL_EXECUTED.ipynb`

Then select **Kernel → Restart & Run All** (or **Run All**) to reproduce the notebook outputs.

## Reproducibility notes

The notebook expects `heart.csv` to be in the same repository directory as the notebook. No absolute file paths are required.

The workflow includes:

- dataset loading and validation;
- preprocessing;
- Logistic Regression;
- Decision Tree;
- Random Forest;
- XGBoost;
- Naive Bayes;
- K-Nearest Neighbours;
- 5-fold stacking ensemble;
- comparison with the published results;
- proposed improved methodology;
- performance metrics including Accuracy, Precision, Recall, F1-score and AUC;
- confusion matrices and ROC analysis.

## Python environment

The project requires Python 3 and the libraries listed in `requirements.txt`.
