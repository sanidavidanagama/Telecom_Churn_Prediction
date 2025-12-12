# Telecom Churn Prediction

This project was completed as part of the **CM2604 Machine Learning** coursework.

**Student:** S.N. Vidanagama  
**IIT ID:** 20231382  
**RGU ID:** 2425607

**Institution:**  
Informatics Institute of Technology (IIT), affiliated with Robert Gordon University (RGU)

---

This project predicts customer churn for a telecom company using machine learning techniques, covering the full data science workflow: data exploration, feature engineering, model building (Decision Tree, Neural Network), evaluation, and deployment preparation.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Environment Setup](#environment-setup)
- [How to Run](#how-to-run)
- [Data](#data)
- [License](#license)

---

## Project Overview

Customer churn prediction helps telecom companies identify customers likely to leave, enabling targeted retention strategies. This project uses the Telco Customer Churn dataset and applies both classical and deep learning models, with careful feature engineering and evaluation.

---

## Project Structure

```
Telecom_Churn_Prediction/
│
├── data/
│   ├── raw/                # Original dataset
│   └── processed/          # Processed dataset
│
├── notebooks/
│   ├── exploratory_data_analysis.ipynb   # EDA
│   ├── feature_engineering.ipynb         # Feature Eng
│   ├── decision_tree.ipynb               # Decision Tree
│   └── neural_network.ipynb              # Neural Network
│
├── pyproject.toml           # Project dependencies
└── README.md                # Project documentation
```

- **data/raw/**: Contains the original Telco Customer Churn CSV file (included in the repository).
- **data/processed/**: Contains cleaned and encoded datasets for modeling.
- **notebooks/**: Jupyter notebooks for each stage of the workflow.
- **.venv/**: Local Python virtual environment.
- **pyproject.toml**: Dependency specification for reproducibility.

> **Note:** The `hyperband_tunings/` directory is excluded from the repository.

---

## Environment Setup

This project uses [uv](https://github.com/astral-sh/uv) for fast, reliable Python dependency management.

### 1. Clone the repository

```bash
git clone https://github.com/sanidavidanagama/Telecom_Churn_Prediction.git
cd Telecom_Churn_Prediction
```

### 2. Create a virtual environment

```bash
uv .venv
```

### 3. Activate the environment

- **Windows:**
    ```bash
    .venv\Scripts\activate
    ```
- **macOS/Linux:**
    ```bash
    source .venv/bin/activate
    ```

### 4. Install dependencies with uv

```bash
uv sync
```

This will install all required packages as specified in `pyproject.toml`.

---

## How to Run

1. **Open JupyterLab or VS Code**  
     Launch JupyterLab or open the notebooks in VS Code.

2. **Run the notebooks in order:**
     - `exploratory_data_analysis.ipynb`: Data cleaning, EDA, and insights.
     - `feature_engineering.ipynb`: Feature creation, encoding, and scaling.
     - `decision_tree.ipynb`: Decision Tree modeling, pruning, and evaluation.
     - `neural_network.ipynb`: Neural Network modeling, hyperparameter tuning, and evaluation.

3. **Review results and figures**  
     Each notebook contains visualizations and summary findings.

---

## Data

- **Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Location:** The dataset and processed files are included in the repository under `data/raw/` and `data/processed/`.

---

## License

This project is licensed under the terms described in the [LICENSE](LICENSE) file.

