# Project Title: O Level Score Prediction using Machine Learning Algorithms

This project is a assignment of AISG's practice papers from their repository at https://github.com/aisingapore/AIAP-Technical-Assessment-Past-Years-Series

## Contributor: Kenneth Goh(thetruthkenhurt)

## Overview of Folder Structure

/O_level_score_prediction_
|-- notebooks/
| |-- sqlitefilequerytest.ipynb # Main analysis notebook
|-- data/
| |-- processed_data.csv # Raw data file
|-- requirements.txt # Project dependencies
|-- README.md # Project documentation


## Instructions for Executing the Pipeline
To run the analysis pipeline:
1. Ensure Python 3.8+ is installed.
2. Install dependencies: `pip install -r requirements.txt`.
3. Navigate to the `/notebooks` directory.
4. Open `sqlitefilequerytest.ipynb` using Jupyter Notebook or JupyterLab.
5. Run all cells in the notebook to reproduce the analysis.

## Modifying Parameters
Parameters such as model hyperparameters or data file paths can be modified in the designated cells within the Jupyter notebook.

## Pipeline Design and Logical Flow
The pipeline follows these key steps:
1. Data loading and preprocessing.
2. Exploratory Data Analysis (EDA) to understand the dataset.
3. Feature engineering based on EDA insights.
4. Model training including cross-validation.
5. Model evaluation and comparison.

## Key Findings from EDA
- Significant variables identified: `class_size`, `hours_per_week`.
- Relationships observed influenced feature engineering and model choice.

## Feature Processing
| Feature          | Processing Steps         |
|------------------|--------------------------|
| `class_size`     | Normalized               |
| `hours_per_week` | Transformed to log-scale |
| `attendance_rate`| Scaled using MinMax      |

## Model Choice Rationale
- **Random Forest**: Chosen for its ability to handle non-linear data with minimal preprocessing.
- **XGBoost**: Selected for its high performance on structured data and importance scoring feature.

## Model Evaluation
Models were evaluated using the following metrics:
- **RMSE (Root Mean Squared Error)**: Measures the average magnitude of the errors in a set of predictions.
- **R-squared**: Represents the proportion of the variance for the dependent variable that's explained by the independent variables in the model.

Further evaluation details and specific metric scores are available within the notebook.

