# Credit Risk Default Prediction

## Overview
This project implements a machine learning solution for predicting credit risk using the German Credit Dataset. It provides a comprehensive analysis of credit risk factors and develops predictive models to assist in credit decision-making.

## Dataset
The dataset used in this project is the German Credit Dataset, available on [Kaggle](https://www.kaggle.com/datasets/mpwolke/cusersmarildownloadsgermancsv). It contains information about 1000 loan applicants with various features including:
- Credit amount
- Duration of credit
- Purpose of credit
- Age and personal information
- Employment status
- Other relevant credit-related attributes

## Project Structure
```
├── credit_risk_analysis.ipynb    # Exploratory Data Analysis (EDA)
├── credit_risk_modeling.ipynb    # Model Development and Evaluation
├── german.csv                    # Dataset
└── requirements.txt              # Python dependencies
```

## Key Features

### 1. Exploratory Data Analysis (EDA)
- Comprehensive analysis of credit risk factors
- Statistical analysis of customer segments
- Feature correlation analysis
- Visual insights into risk patterns
- Age and employment impact analysis

### 2. Model Development
- Data preprocessing and feature engineering
- Implementation of multiple models:
  - Logistic Regression (baseline)
  - XGBoost (advanced model)
- Handling class imbalance
- Feature importance analysis

### 3. Risk Assessment
- SHAP (SHapley Additive exPlanations) value analysis
- Risk segmentation strategies
- Credit amount vs. duration analysis
- Employment stability impact

### 4. Business Insights
- Risk-based pricing recommendations
- Customer segmentation strategies
- Credit policy suggestions
- Portfolio management insights

## Model Performance

Our models achieve the following performance metrics:

- XGBoost Model:
  - Accuracy: ~77.5%
  - Precision: ~81% for good credit risk
  - ROC-AUC Score: ~76%

- Key Findings:
  - Better performance in identifying good credit risks
  - Balanced approach between risk identification and approval
  - Strong predictive power for medium to high-risk cases

## Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/hosseinmang/Credit-Risk-Default-Prediction.git
cd Credit-Risk-Default-Prediction
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Run the notebooks in order:
   - First: `credit_risk_analysis.ipynb` for EDA
   - Second: `credit_risk_modeling.ipynb` for modeling

## Key Insights

1. **Credit Duration and Amount**:
   - Longer credit durations correlate with higher risk
   - Medium-term loans with moderate amounts show optimal risk-return profile
   - Clear relationship between amount and default probability

2. **Age and Experience**:
   - Middle-aged borrowers (35-45) show lowest risk profile
   - Employment stability significantly impacts credit risk
   - Age-based risk patterns provide segmentation opportunities

3. **Risk Segmentation**:
   - Low Risk: Short-term, moderate amounts, stable employment
   - Medium Risk: Medium-term, higher amounts
   - High Risk: Long-term, very high amounts, or employment instability

## Business Applications

This project can be used for:
- Credit risk assessment
- Loan approval automation
- Risk-based pricing
- Portfolio management
- Customer segmentation
- Credit policy development

## Tools & Technologies
- Python 3.x
- Key Libraries:
  - pandas
  - numpy
  - scikit-learn
  - xgboost
  - shap
  - matplotlib
  - seaborn

## Future Enhancements
- Implementation of deep learning models
- Real-time risk assessment API
- Integration with banking systems
- Enhanced feature engineering
- Additional risk metrics

## Contributing
Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is open source and available under the MIT License.

## Acknowledgments
- Dataset source: [German Credit Dataset on Kaggle](https://www.kaggle.com/datasets/mpwolke/cusersmarildownloadsgermancsv)
- SHAP library for model interpretability
- XGBoost community for the gradient boosting framework

## Contact
For any queries or discussions, please open an issue in the GitHub repository.