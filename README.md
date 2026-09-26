# Telco Customer Churn Prediction & Business Insights

A machine learning project designed to predict customer churn for a telecommunications company using the IBM Telco dataset. This project emphasizes robust preprocessing, handling severe class imbalance, maximizing churn recall, and extracting actionable business drivers to improve retention strategies.

---

## 🚀 Project Overview

Customer churn is a critical metric for subscription-based businesses. Acquiring new customers is significantly more expensive than retaining existing ones. This project builds an end-to-end classification pipeline to identify customers at high risk of churning, allowing businesses to proactively intervene.

---

## 📂 Project Structure

```text
Customer Churn Prediction/
│
├── data/                  # Raw and processed datasets (IBM Telco Customer Churn CSV)
├── models/                # Serialized model artifacts (.sav pipelines)
├── notebooks/             # Jupyter notebooks for EDA, experimentation, and modeling
├── outputs/               # Exported visualizations and evaluation charts (300 DPI)
├── venv/                  # Python virtual environment
├── .gitignore             # Git ignore file
├── customer_churn_prediction_plan.md # Project planning and architecture notes
├── requirements.txt       # Core project dependencies
└── README.md              # Project documentation
```

⚙️ Data Preprocessing & Engineering
Data Cleaning: Handled missing values in TotalCharges by coercing parsing errors to numeric and filling nulls for brand-new customers with 0.

Preprocessing Pipeline: Built a robust scikit-learn ColumnTransformer to handle feature transformations dynamically:

Numerical Features: Imputation and scaling.

Categorical Features: One-Hot Encoding to expand categorical variables (such as InternetService and PaymentMethod) into clean numerical matrices.

🤖 Modeling & Evaluation
Two primary models were built, tuned, and evaluated:

Logistic Regression (Champion Model): Selected as the champion model due to its exceptional interpretability and high churn recall (83%).

Random Forest Classifier: Evaluated as a non-linear baseline.

Key Modeling Strategies:

Configured both models with class_weight='balanced' to effectively combat the inherent class imbalance in churn datasets.

Prioritized Recall over raw accuracy to ensure the business catches as many potential churners as possible, minimizing false negatives.

Serialized the final pipelines using joblib into the models/ directory for seamless deployment.

💡 Key Business Insights
By extracting and analyzing feature coefficients from the Logistic Regression model, several critical retention drivers were uncovered:

High-Risk Churn Drivers: Customers utilizing Fiber optic internet service and electronic check payment methods show a significantly higher propensity to churn.

Retention Drivers: Long-term contracts (one or two years), automatic payment methods, and supplementary services like online security and technical support heavily protect customer retention.

🛠️ Installation & Setup
Clone the repository and navigate to the project root.

Create and activate your virtual environment:

Bash

```
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

Install the required dependencies:

Bash

```
pip install -r requirements.txt
```
