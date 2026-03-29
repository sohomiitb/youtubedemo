# Bank Customer Churn Model Demo

This project demonstrates an end-to-end pipeline for modeling customer churn using a synthetic bank dataset. The workflow covers data generation, handling class imbalance, model training, Bayesian prior correction, and evaluation.

## Features
- **Synthetic Data Generation:** Creates a realistic, imbalanced bank customer churn dataset.
- **Class Imbalance Handling:** Downsamples the majority class to a 9:1 ratio for training.
- **Model Training:** Trains a logistic regression model with preprocessing (scaling and one-hot encoding).
- **Bayesian Prior Correction:** Adjusts predicted probabilities to account for the true population prior.
- **Evaluation:** Provides metrics including ROC AUC, PR AUC, confusion matrix, and classification report.
- **CSV Export:** Saves sampled training data and scored test set to CSV files.

## Usage
1. **Open the Notebook**: `chunmodel.ipynb` in VS Code or Jupyter.
2. **Run All Cells**: The notebook will generate data, train the model, evaluate, and save results.
3. **Outputs**:
   - `bank_customer_churn_train_9_to_1.csv`: Downsampled training data (9:1 ratio).
   - `bank_customer_churn_scored_test_set.csv`: Test set with predicted probabilities and classes.

## Main Functions
- `generate_bank_churn_data`: Generates the synthetic dataset.
- `downsample_to_ratio`: Downsamples the majority class.
- `build_logistic_model`: Builds a preprocessing + logistic regression pipeline.
- `adjust_probabilities_for_prior_shift`: Applies Bayesian prior correction.
- `evaluate_predictions`: Evaluates model predictions.
- `run_churn_model_demo`: Runs the full pipeline and returns results.

## Requirements
- Python 3.7+
- pandas
- numpy
- scikit-learn

Install dependencies with:
```bash
pip install pandas numpy scikit-learn
```

## License
MIT License
