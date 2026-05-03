# particle-physics-event-classification

## Problem Statement
Classify particle physics events into **Signal (s)** and **Background (b)** 
using machine learning techniques on data derived from particle experiments.

## Dataset
- 250,001 events | 33 features
- Missing values encoded as -999
- Target: Signal (s) / Background (b)

## Models Used
| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | ~0.78 | ~0.85 |
| Decision Tree | ~0.82 | ~0.82 |
| Random Forest | ~0.87 | ~0.93 |
| Gradient Boosting | ~0.86 | ~0.92 |

## Key Steps
1. Data Collection & Loading
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing (missing values, encoding, scaling)
4. Model Training (4 models)
5. Evaluation (Accuracy, ROC-AUC, Confusion Matrix)
6. Hyperparameter Tuning (GridSearchCV)
7. Feature Importance Analysis

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## How to Run
1. Clone the repo
2. Place `Data_science_dataset.csv` in the same folder
3. Open `Particle_Physics_Project_Improved.ipynb` in Jupyter
4. Run all cells
