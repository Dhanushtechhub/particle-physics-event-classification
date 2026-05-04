# Particle Physics Event Classification

## Problem Statement
Classify particle physics events into **Signal (s)** and **Background (b)** 
using machine learning techniques on data derived from particle experiments.

## Dataset
- 250,000 events | 33 features
- Missing values encoded as -999
- Target: Signal (s) / Background (b)
- Download dataset: [Click Here](paste your Google Drive CSV link here)

## Models Used
| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | 0.7385 | 0.7985 |
| Decision Tree | 0.82 | 0.82 |
| Random Forest (Tuned) | 0.8349 | 0.9021 |
| Gradient Boosting | 0.86 | 0.92 |

## Key Steps
1. Data Collection & Loading
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing (missing values, encoding, scaling)
4. Model Training (4 models)
5. Evaluation (Accuracy, ROC-AUC, Confusion Matrix)
6. Hyperparameter Tuning (RandomizedSearchCV)
7. Feature Importance Analysis

## Top 5 Important Features
| Feature | Importance |
|---------|------------|
| DER_mass_MMC | 0.146 |
| DER_mass_transverse_met_lep | 0.114 |
| DER_mass_vis | 0.086 |
| PRI_tau_pt | 0.062 |
| DER_met_phi_centrality | 0.060 |

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## How to Run
1. Clone the repo
2. Download the dataset from the link above
3. Place `Data_science_dataset.csv` in the same folder as the notebook
4. Open `Particle_Physics_Project.ipynb` in Jupyter
5. Run all cells

## Results
Best model: **Tuned Random Forest**
- Accuracy: 0.8349
- ROC-AUC: 0.9021

## Future Work
- Try XGBoost / LightGBM for further improvement
- Use AMS (Approximate Median Significance) metric with event weights
- Apply SHAP values for deeper explainability
