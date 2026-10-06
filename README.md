# MLflow Customer Churn Project

An MLOps learning project for customer-churn classification with experiment tracking through MLflow.

## Current repository state

The GitHub repository currently contains the project scaffold, dependency manifest, and ignore rules, but the main implementation files used during local development are **not currently committed to the main branch**.

Because of that, this README intentionally does not pretend the repository contains executable training, evaluation, or API code. Humans have somehow survived for millennia without honest READMEs, but recruiters tend to notice when the documentation describes files that do not exist.

## Intended workflow

~~~text
Raw Customer Churn Data
        ↓
Data Download
        ↓
Preprocessing / Feature Engineering
        ↓
Train / Test Split
        ↓
Model Training
   ┌────┴────┐
   ↓         ↓
Logistic   Random
Regression Forest
   └────┬────┘
        ↓
Evaluation
        ↓
MLflow Experiment Tracking
        ↓
Metrics / Model Comparison
~~~

## Planned project components

- Customer-churn dataset download and preparation
- Feature preprocessing
- Logistic Regression baseline
- Random Forest comparison
- Accuracy, precision, recall, and F1 evaluation
- MLflow experiment tracking
- Local MLflow backend using SQLite during development
- Optional API layer for serving predictions

## Technology

- Python
- Pandas
- Scikit-learn
- MLflow
- SQLite
- FastAPI / Uvicorn for the API layer when the serving component is present

## Local development

The dependency manifest is retained from the development environment. Once the source implementation is committed, the expected workflow will be:

~~~bash
python -m venv .venv
~~~

Windows:

~~~powershell
.\.venv\Scripts\Activate.ps1
~~~

Install dependencies:

~~~bash
pip install -r requirements.txt
~~~

Then run the project's data preparation, training, evaluation, and MLflow commands documented alongside the committed source files.

## Important

Before using this repository as a portfolio project, commit the actual `src/`, `api/`, and `tests/` implementation files from the working local project. The current GitHub version is a scaffold, not a complete portfolio-ready implementation.

## Author

**Subham Dey**
