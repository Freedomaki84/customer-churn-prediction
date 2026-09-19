# Plan 1: Customer Churn Prediction (Supervised Machine Learning)

## Project Overview & Methodology
* **Objective:** Build an end-to-end machine learning model that predicts whether a customer will churn based on historical usage and account data.
* **Core Rule:** **You (the user) will write 100% of the code.** My role is strictly to provide conceptual explanations, architectural guidance, debugging advice, and step-by-step instructions. I will not write code snippets for you.
* **Tech Stack:** Python, Pandas, Scikit-Learn, Matplotlib/Seaborn, Jupyter Notebook.

## Step-by-Step Execution Plan (Instructions for You)

### Phase 1: Environment Setup & Dataset Acquisition
* **Your Task:** Set up your local Python environment and Jupyter Notebook. Download the Telco Customer Churn dataset from Kaggle and load it into a Pandas DataFrame.
* **My Coaching Role:** I will guide you on how to structure your notebook, check data types, and inspect missing values without giving you the code.

### Phase 2: Exploratory Data Analysis (EDA) & Data Cleaning
* **Your Task:** Write the data cleaning code to handle missing values, encode categorical variables, and scale numerical features. Create visual plots (churn distribution, correlation matrices) using Matplotlib/Seaborn.
* **My Coaching Role:** I will explain the theory behind encoding and scaling, and help you interpret your visualizations so you know what cleaning steps to implement yourself.

### Phase 3: Baseline & Iterative Model Training
* **Your Task:** Split your data into training and testing sets. Write the code to train a baseline model (e.g., Logistic Regression) and an improved model (e.g., Random Forest).
* **My Coaching Role:** I will explain how train/test splits work and outline the conceptual steps for fitting models using Scikit-Learn so you can write the logic yourself.

### Phase 4: Model Evaluation & Feature Importance
* **Your Task:** Evaluate your models using precision, recall, F1-score, and ROC-AUC curves. Extract and plot feature importances from your tree-based model.
* **My Coaching Role:** I will help you interpret evaluation metrics and guide you on how to extract feature importance attributes independently.

### Phase 5: Business Interpretation & Documentation
* **Your Task:** Translate your model's findings into plain-language business insights and write a comprehensive README file for your GitHub repository.
* **My Coaching Role:** I will review your written summaries and suggest how to frame your results effectively for recruiters.