# Customer Churn Prediction: End-to-End ML Pipeline

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.5.3-green)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2.2-red)
![SHAP](https://img.shields.io/badge/SHAP-0.41.0-orange)

## Project Overview

This repository contains an end-to-end machine learning pipeline for predicting customer churn in a telecommunications company. The project demonstrates how to build a robust predictive model that not only forecasts which customers are likely to leave, but also provides actionable insights for retention strategies.

### Business Problem

Customer churn - the loss of clients or customers - is one of the most significant challenges faced by subscription-based businesses. In the telecommunications industry:
- Acquiring a new customer can cost 5-25 times more than retaining an existing one
- A 5% increase in customer retention can increase profits by 25-95%

This project addresses this challenge by developing a system that:
1. Accurately predicts which customers are at high risk of churning
2. Identifies key factors contributing to churn
3. Enables targeted retention strategies through customer segmentation
4. Quantifies the potential financial impact of retention efforts

## Key Features

- **Comprehensive Data Analysis**: In-depth exploration of customer demographics, service usage, and contract details
- **Advanced Feature Engineering**: Creation of custom features to capture complex relationships
- **Model Development & Evaluation**: Implementation and comparison of multiple ML algorithms with hyperparameter tuning
- **Interpretable AI**: Use of SHAP values and feature importance techniques to explain model predictions
- **Customer Segmentation**: Risk-based segmentation and clustering for targeted retention strategies
- **Business Recommendations**: Actionable insights with expected ROI calculations

## Main Results

- Achieved **84.65% ROC AUC** on the test dataset
- Identified key churn drivers:
  1. Contract type (month-to-month contracts have 15x higher churn than two-year contracts)
  2. Customer tenure (highest risk in first 12 months)
  3. Internet service type (fiber optic users churn at 2.2x the rate of DSL users)
  4. Payment method (electronic check users have 2.7x higher churn than automatic payments)
  5. Technical support services (lack of technical support correlates with 2.7x higher churn)

- Customer segmentation revealed 4 distinct clusters with different retention strategies:
  1. **Loyal DSL users** (8% churn rate): Reward loyalty, cross-sell premium services
  2. **New Fiber Optic users** (57% churn rate): Improve onboarding, offer tech support
  3. **High-value long-term customers** (18% churn rate): Service quality focus, loyalty rewards
  4. **New budget customers** (35% churn rate): Early engagement, education on services

- Financial impact: Calculated potential annual savings of $145,248 from just a 10% reduction in churn rate

## Repository Contents

- `Customer_Churn_Prediction.ipynb`: Jupyter notebook with the full analysis and model development
- `data/`: Directory containing the dataset used in the analysis
- `models/`: Saved model files for deployment
- `visualizations/`: Key plots and charts from the analysis
- `requirements.txt`: Required Python packages

## Installation & Usage

1. Clone this repository:
```
git clone https://github.com/Khubaibakramshirani/customer-churn-prediction.git
```

2. Install required packages:
```
pip install -r requirements.txt
```

3. Run the Jupyter notebook:
```
jupyter notebook Customer_Churn_Prediction.ipynb
```

## Model Deployment

The model can be deployed as an API using Flask. The implementation blueprint is included in the notebook, covering:

1. Model serialization with pickle
2. API endpoint creation for individual customer prediction
3. Integration with CRM systems for automated risk scoring

## Future Work

- Implement automatic model retraining pipeline
- Add time-series analysis for churn prediction
- Explore deep learning approaches for improved accuracy
- Develop a dashboard for business users to interact with predictions

## Acknowledgements

- Dataset: IBM Telco Customer Churn dataset

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For any questions or feedback, please reach out to:
- Email: khubaibshirani@gmail.com
- LinkedIn: (https://www.linkedin.com/in/khubaib-akram/)
- GitHub: (https://github.com/Khubaibakramshirani)
