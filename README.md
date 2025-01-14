# class-imbalance-counterfactual-augmentation

# Project Overview :
This project explores the use of counterfactual data augmentation to address class imbalance in datasets. By generating synthetic samples for the minority class and leveraging explainable AI (SHAP and LIME), we improve model performance and interpretability.

# Key Features
Counterfactual data augmentation for handling class imbalance.
SHAP and LIME for feature importance analysis.
Pre- and post-augmentation comparisons of model performance.

# Project Workflow
Train the model on the imbalanced dataset.
Use SHAP and LIME for feature analysis.
Perform counterfactual data augmentation.
Retrain the model with the balanced dataset.
Compare pre- and post-augmentation results.

# How to Run
1. Clone the repository : cd class-imbalance-counterfactual-augmentation

2. Install dependencies : pip install -r requirements.txt

3. Perform SHAP and LIME analysis : python src/explainability.py

# Results
Improved minority class performance after augmentation.
Visualizations of feature importance (SHAP and LIME).

# Directory Structure
class-imbalance-counterfactual-augmentation/
├── data/                     # Raw and processed datasets
│   ├── original/             # Original dataset
│   ├── augmented/            # Augmented dataset (synthetic data)
├── notebooks/                # Jupyter notebooks for analysis
│   ├── data_augmentation_model_training.ipynb  # Notebook for augmentation and training
│   └── exploratory_analysis.ipynb             # Notebook for exploratory data analysis
├── src/                      # Source code files
│   ├── augmentation.py       # Script for data augmentation
│   ├── train_model.py        # Script for model training
│   ├── explainability.py     # SHAP and LIME analysis
│   └── utils.py              # Helper functions and utilities
├── results/                  # Results and outputs
│   ├── metrics/              # Model performance metrics
│   ├── visualizations/       # SHAP and LIME plots, decision boundaries
├── tests/                    # Unit and integration tests
│   ├── test_augmentation.py  # Tests for augmentation script
│   ├── test_model.py         # Tests for training script
├── LICENSE                   # License file (e.g., MIT License)
├── README.md                 # Project overview and instructions
├── requirements.txt          # Python dependencies
├── .gitignore                # Files and folders to ignore
└── CONTRIBUTING.md           # Guidelines for contributors

# Example Visualizations
Upload SHAP/LIME visualizations, confusion matrices, and performance metrics in the results/visualizations folder. Include these in the README under Results using markdown syntax:

### Feature Importance (SHAP)
![SHAP Summary Plot](results/visualizations/shap_summary.png)

### Model Performance
| Metric         | Pre-Augmentation | Post-Augmentation |
|----------------|------------------|-------------------|
| Precision      | 0.75             | 0.88              |
| Recall         | 0.65             | 0.85              |
| F1-Score       | 0.69             | 0.87              |



