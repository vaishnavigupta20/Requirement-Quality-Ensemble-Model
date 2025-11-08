# Requirement Quality Ensemble Model

## Project Overview
This project implements an ensemble machine learning system to predict the quality of requirement statements. Classification categories are: **Ambiguous**, **Complete**, and **Inconsistent**.

## Features
- Manual annotation and preprocessing of requirement sentences.
- Model training with SVM, Random Forest, and Gradient Boosting.
- Ensemble methods using stacking classifiers.
- Evaluation using F1-score and classification metrics.
- Predicts the quality of new requirement sentences.

## Workflow
1. Data Preprocessing: Converts all characters to lowercase, removes all non-alphabetic characters, strips extra whitespaces from beginning and the end, TF-IDF vectorization.
2. Model Training: Trains three base classifiers—SVM, Random Forest, and Gradient Boosting.
3. Ensemble Training: Combines base models using stacking.
4. Performance Evaluation: Reports F1-score improvement and detailed classification results.

## Getting Started
1. Clone the repository.
2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```
3. Run the Jupyter Notebook (`aiml_ensemble.ipynb`) to view and test the results.

## Input
- Manually annotated dataset with at least 200 requirement sentences across the target classes.

## Output
- Quality predictor system prototype with evaluation plots, metrics, and example predictions.

## Files Included
- `aiml_ensemble.ipynb.ipynb`: Main notebook.
- `requirements.txt`: List of required Python libraries.
