> 📖 🇪🇸 También disponible en español: [README.es.md](README.es.md)

# Personal Expense Analysis & Prediction Model

[![Language](https://img.shields.io/badge/code-Python-blue.svg?logo=python&logoColor=white)](https://python.org/)
[![Framework](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Colab](https://img.shields.io/badge/Google-Colab-orange.svg?logo=GoogleColab&logoColor=white)](https://scikit-learn.org/)
[![ML Library](https://img.shields.io/badge/Field-Machine%20Learning-red.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

## Project Overview

This data science project tackles personal finance management through predictive modeling. Using machine learning techniques, I developed a system that predicts activity costs based on multiple variables including budget allocation, activity type, time of day, and number of participants. The project demonstrates the practical application of the CRISP-DM methodology to solve real-world financial planning challenges.

**Problem Statement:** Can we accurately predict the cost of personal activities based on budgetary and contextual factors, and use these insights to improve financial decision-making?

## Key Features

- **Predictive Cost Modeling**: Linear regression model achieving 85% accuracy (R² = 0.85)
- **Comprehensive Data Analysis**: Statistical analysis of 285+ expense records across 89 days
- **Financial Insights**: Automated calculation of savings patterns and budget optimization recommendations
- **Data Visualization**: Clear graphical comparisons between predicted and actual costs

## Technical Implementation

### Technologies Used
- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning implementation
- **Matplotlib**: Data visualization
- **Jupyter Notebooks**: Interactive development environment
- **Google Colab**: Cloud-based execution platform

### Programming Concepts Applied

1. **Data Preprocessing & Validation**
   - Systematic handling of missing values using `dropna()` 
   - Data type validation and format standardization
   - Feature selection through column subsetting (`iloc[:,3:9]`)

2. **Statistical Modeling**
   - Linear regression implementation with train-test split (80/20)
   - Coefficient analysis for feature importance assessment
   - Model evaluation using R² score and residual analysis

3. **Error Handling & Data Quality**
   - Null value detection and cleanup procedures
   - Data integrity checks before and after preprocessing
   - Iterative model refinement through multiple runs

4. **Algorithmic Problem-Solving**
   - Feature engineering for categorical variables (activity type, time moment)
   - Multi-variable prediction using budget, time, type, moment, and group size
   - Financial metrics calculation (savings rate, goal achievement timeline)

## Methodology: CRISP-DM Framework

### Phase 1: Business Understanding
- **Objective**: Predict personal activity costs for improved budget planning
- **Success Criteria**: Develop a model that explains >80% of cost variance
- **Stakeholder**: Personal financial management optimization

### Phase 2: Data Understanding
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QB_lH_D7s-Vi4gmNGMjiLfeD8VPEAWVw?usp=sharing)
- **Data Sources**: Personal expense records (285 activities, 89 days)
- **Key Variables**: Budget, Cost, Activity Type, Time Moment, Group Size
- **Data Quality**: Identified and addressed missing values in cost records

### Phase 3: Data Preparation  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1oP9cLpB8nw0WeR2r1aw2ijqvSLAy-brl?usp=sharing)
- **Data Selection**: Focused on 6 core attributes most relevant to cost prediction
- **Cleaning**: Removed records with null values to ensure model reliability
- **Feature Engineering**: Prepared categorical variables for regression analysis
- **Training Split**: 80% training, 20% testing for robust validation

### Phase 4: Data Modeling
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jaAr7F8DuQHmI8Q75R8YxRFWM5c8gQR5?usp=sharing)
- **Algorithm**: Linear Regression (scikit-learn implementation)
- **Performance**: R² = 0.85, indicating strong predictive capability
- **Validation**: Residual analysis and visual comparison of predicted vs. actual costs
- **Iteration**: Three modeling attempts to optimize parameters and data quality

## Key Results

- **Model Accuracy**: 85% of cost variance explained by the model
- **Financial Insights**: 
  - Total expenses tracked: $71,630
  - Total savings achieved: $17,830  
  - Average daily savings: $200
  - Wishlist goal achievement: ~5 days for $1,000 item
- **Budget Optimization**: Identified high-cost activity patterns for targeted reduction

## Learning Outcomes Demonstrated

**SEG0502 - Problem Solving with Valid Methodologies**: Applied the CRISP-DM framework systematically to address a real-world financial management challenge, demonstrating rigorous methodology from business understanding through deployment.

**SEG0701 - Strategic Digital Technology Use**: Leveraged Python, Jupyter notebooks, and Google Colab to create value through data-driven insights, transforming raw expense data into actionable financial intelligence.

**SEG0702 - Technology Evaluation and Implementation**: Evaluated multiple approaches for data preprocessing and modeling, selecting linear regression based on interpretability requirements and implementing iterative improvements based on performance metrics.

## Final Reflection

This project significantly expanded my understanding of applied data science in personal finance, providing hands-on experience with the complete CRISP-DM lifecycle from problem formulation to actionable insights. The most challenging aspect was ensuring data quality during preprocessing—systematically identifying and handling missing values taught me the critical importance of clean data in machine learning success.

The modeling phase was particularly rewarding, allowing me to witness abstract statistical concepts translate into practical predictions about spending behavior. This work strengthened my Python programming skills, especially in data manipulation with pandas and visualization with matplotlib, while teaching me to think algorithmically about real-world problems and validate solutions through rigorous testing.

Looking forward, I plan to expand this work by incorporating time-series analysis for seasonal spending patterns and exploring ensemble methods to improve prediction accuracy.
