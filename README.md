# epidemic_app
Epidemic Pattern Analyzer
A comprehensive Streamlit web application that analyzes epidemic patterns using machine learning and SIR (Susceptible-Infected-Recovered) models. The application predicts disease similarity based on epidemic parameters and provides detailed analysis with real-world disease comparisons.

Features
Disease Analysis
10+ Diseases Supported: Pertussis, Mumps, Measles, Rubella, Tetanus, Typhoid, Polio, Diphtheria, Meningococcal, Yellow Fever

Real Disease Data: Historical case data from WHO and health organizations

Disease Information: R0 ranges, incubation periods, and descriptions

# Machine Learning Models
Multiple Classifiers:

Random Forest

Gradient Boosting

XGBoost

LightGBM

SVM

Neural Networks (MLP)

Decision Trees

Naive Bayes

Ensemble Methods: Voting and Stacking classifiers

Cross-Validation: Robust model evaluation

Feature Engineering: Advanced statistical feature extraction

# SIR Modeling
Interactive Parameters: Adjust population, infection rates, and recovery rates

Real-time Simulation: Dynamic SIR curve generation

R0 Calculation: Automatic basic reproduction number computation

Visualization: Interactive Plotly charts

# Pattern Matching
Similarity Analysis: Compare simulated epidemics with real disease patterns

Country-level Data: Find countries with similar historical outbreaks

Confidence Scoring: Combined AI probability and R0 matching

Installation
Prerequisites
Python 3.8+

pip package manager

# Step 1: Clone the Repository
bash
git clone https://github.com/yourusername/epidemic-pattern-analyzer.git
cd epidemic-pattern-analyzer
#Step 2: Install Dependencies
bash
pip install -r requirements.txt
Required packages:
streamlit
pandas
numpy
matplotlib
plotly
scipy
scikit-learn
xgboost
lightgbm
openpyxl
# Step 3: Prepare Data Files
Create a data directory and add the following Excel files:
Pertussis_reported_cases_and_incidence_2025_18_11_13_34_UTC_1.xlsx
Mumps reported cases and incidence 2025-18-11 13-36 UTC.xlsx
Measles reported cases and incidence 2025-18-11 13-23 UTC.xlsx
Rubella reported cases and incidence 2025-18-11 13-53 UTC.xlsx
Tetanus reported cases and incidence 2025-18-11 13-22 UTC.xlsx
Typhoid reported cases and incidence 2025-18-11 13-25 UTC.xlsx
Poliomyelitis_reported_cases_and_incidence_2025_18_11_13_31_UTC.xlsx
Diphtheria_reported_cases_and_incidence_2025_18_11_14_00_UTC.xlsx
Invasive_meningococcal_disease_reported_cases_and_incidence_2025.xlsx
Yellow_Fever_YF_reported_cases_and_incidence_2025_18_11_13_40_UTC.xlsx

# Step 4: Run the Application
streamlit run app.py
The application will open in your default web browser at http://localhost:8501.

# Usage
1. Setting Epidemic Parameters
Total Population (N): Size of the population being modeled
Initial States: Set initial Susceptible (S0), Infected (I0), and Recovered (R0) populations
Infection Rate (β): Controls how quickly the disease spreads
Recovery Rate (γ): Determines how quickly people recover
2. Model Selection
Choose from multiple trained ML models
Ensemble models (Voting/Stacking) recommended for best performance
View model accuracy scores for informed selection
3. Analysis Results
SIR Simulation: Visualize the epidemic curve
Top Predictions: See which real diseases match your parameters
Confidence Scores: Combined AI probability and R0 matching
Similar Patterns: Find countries with historical similarities

# 4. Export Results
Download predictions as CSV files

Save analysis for further study

#Project Structure
epidemic-pattern-analyzer/
│
├── app.py                 # Main application file
├── data/                  # Disease data directory
│   ├── Pertussis_reported_cases_and_incidence_*.xlsx
│   ├── Mumps_reported_cases_and_incidence_*.xlsx
│   └── ... (other disease files)
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
Data Sources
The application uses historical disease data from:

World Health Organization (WHO)

Centers for Disease Control and Prevention (CDC)

Global health monitoring systems

Model Performance
The application trains multiple machine learning models with:

Feature Engineering: 12 advanced statistical features

Cross-Validation: 3-fold cross-validation for robust evaluation

Ensemble Methods: Combined predictions for improved accuracy

Data Cleaning: Robust handling of missing and noisy data

# Key Features
Advanced Feature Extraction
Statistical measures (mean, std, min, max, median)

Trend analysis and slope calculation

Percentage changes and volatility

Distribution shape analysis

Non-zero ratio and coefficient of variation

Robust Data Processing
Automatic data validation and cleaning

Handling of regional/global data aggregation

Multi-year data analysis (2015-2024 focus)

Country-level granularity

Interactive Visualization
Real-time SIR curve updates

Interactive prediction charts

Model performance comparisons

Similar pattern discovery

Contributing
Contributions are welcome! Please feel free to submit pull requests for:

Additional disease data

Improved machine learning models

Enhanced visualization features

Bug fixes and performance improvements

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
World Health Organization for disease data

Scikit-learn, XGBoost, and LightGBM teams for ML libraries

Plotly for interactive visualizations

Streamlit for the web framework
