# Disease Profile Prediction - CSE437 Data Science Project

A comprehensive machine learning project that predicts future disease profiles for countries based on historical mortality data from 1990-2019. The project uses epidemiological transition theory to classify countries into different disease burden categories and predicts their future health patterns using Random Forest classification.

## 🌟 Project Overview

This project analyzes global mortality data to understand how countries transition through different epidemiological stages, from infectious disease dominance to chronic disease prevalence. It predicts future disease profiles (2010-2019) based on historical patterns (1990-2009) using advanced machine learning techniques.

## 📊 Dataset Information

### Data Source

- **Global Burden of Disease Study** - Cause of deaths dataset
- **Time Period**: 1990-2019 (30 years)
- **Geographic Coverage**: 204 countries and territories
- **Data Points**: 6,120 country-year observations
- **Features**: 31 cause-of-death categories

### Key Statistics

- **Total Deaths Recorded**: 1.47 billion deaths
- **Average Deaths per Country per Year**: 239,891
- **Data Quality**: No missing values, no negative death counts
- **Temporal Split**: 1990-2009 (training), 2010-2019 (prediction)

## 🎯 Problem Statement

Predict future disease profiles for countries based on their historical mortality patterns, enabling:

- **Public Health Planning**: Anticipate future healthcare needs
- **Resource Allocation**: Optimize medical infrastructure investment
- **Policy Development**: Inform health policy decisions
- **Epidemiological Understanding**: Study disease transition patterns

## 🔬 Methodology

### 1. Data Preprocessing

- **Temporal Split**: Historical (1990-2009) vs Future (2010-2019) periods
- **Feature Engineering**: Created 8 temporal features from historical data
- **Target Classification**: 3 future disease profile categories

### 2. Feature Engineering

- **Historical Development Proxy**: Chronic vs infectious disease ratios
- **Healthcare Quality Proxy**: Preventable death rates
- **Age Structure Proxy**: Elderly vs young population disease patterns
- **Violence Proxy**: Conflict and violence-related deaths
- **Environmental Proxy**: Tropical disease burden
- **Scale Features**: Population size and mortality diversity measures

### 3. Target Classification

- **Chronic_Dominant_Future**: Fully transitioned to chronic diseases
- **Infectious_Dominant_Future**: Early stage with infectious burden
- **Transitional_Future**: Mixed chronic and infectious patterns

### 4. Machine Learning Pipeline

- **Algorithm**: Random Forest Classifier
- **Hyperparameter Tuning**: Grid Search with 5-fold CV
- **Evaluation**: Stratified train/validation/test split (60/20/20)
- **Metrics**: Accuracy, Balanced Accuracy, Precision, F1-Score

## 🛠️ Technical Implementation

### Core Technologies

- **Python 3.x** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Scikit-learn** - Machine learning algorithms
- **Matplotlib/Seaborn** - Data visualization

### Key Libraries

- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **scikit-learn** - Machine learning algorithms
- **matplotlib** - Data visualization
- **seaborn** - Statistical data visualization
- **datetime** - Date and time handling

### Data Processing Pipeline

1. **Data Loading**: CSV file processing and validation
2. **Temporal Analysis**: Historical vs future period analysis
3. **Feature Engineering**: 8 temporal features creation
4. **Target Classification**: 3-category disease profile classification
5. **Model Training**: Random Forest with hyperparameter tuning
6. **Evaluation**: Comprehensive performance assessment

## 📈 Results & Performance

### Model Performance

- **Test Accuracy**: 63.4%
- **Test Balanced Accuracy**: 67.8%
- **Test Precision (weighted)**: 65.2%
- **Test F1-Score (weighted)**: 63.2%

### Feature Importance Analysis

1. **Historical Development Proxy** (32.4%) - Most important predictor
2. **Historical Deaths Per Million** (25.5%) - Population scale factor
3. **Historical Age Structure Proxy** (17.7%) - Demographic patterns
4. **Historical Environmental Proxy** (9.2%) - Tropical disease burden
5. **Historical Violence Proxy** (7.0%) - Conflict-related deaths

### Future Disease Profile Distribution

- **Chronic Dominant Future**: 86 countries (42.2%)
- **Transitional Future**: 79 countries (38.7%)
- **Infectious Dominant Future**: 39 countries (19.1%)

## 📁 Project Structure

```
cse437-project/
├── project.ipynb              # Main Jupyter notebook
├── cause_of_deaths.csv        # Dataset
├── requirements.txt           # Python dependencies
├── Group_17.pdf              # Project report
├── disease_profile_analysis.png # Visualization output
├── X_train.csv               # Training features
├── X_validation.csv          # Validation features
├── X_test.csv                # Test features
├── y_train.csv               # Training labels
├── y_validation.csv          # Validation labels
└── y_test.csv                # Test labels
```

## 🚀 Installation & Setup

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook
- Required Python packages

### Installation Steps

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd cse437-project
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook project.ipynb
   ```

## 📊 Key Findings

### Global Mortality Patterns

- **Top Cause**: Cardiovascular Diseases (30.5% of all deaths)
- **Second Cause**: Neoplasms (15.6% of all deaths)
- **Geographic Distribution**: China and India account for 34% of global deaths

### Epidemiological Transition

- **Developed Countries**: Predominantly chronic disease burden
- **Developing Countries**: Mixed infectious and chronic patterns
- **Least Developed**: High infectious disease burden

### Predictive Insights

- Historical chronic/infectious disease ratios are the strongest predictor
- Population scale significantly influences future disease patterns
- Age structure and environmental factors play important roles

## 🎯Project Summary

### Project Title

**Disease Profile Prediction - Machine Learning for Public Health**

### Project Description

Developed a comprehensive machine learning system to predict future disease profiles for 204 countries based on historical mortality data from 1990-2019. The project uses epidemiological transition theory and Random Forest classification to predict whether countries will have chronic-dominant, infectious-dominant, or transitional disease patterns in the future.

### Key Achievements

- **Data Analysis**: Processed 1.47 billion death records across 204 countries over 30 years
- **Feature Engineering**: Created 8 temporal features capturing historical disease patterns
- **Machine Learning**: Implemented Random Forest with hyperparameter tuning achieving 63.4% accuracy
- **Epidemiological Insights**: Identified key predictors of disease transition patterns
- **Visualization**: Created comprehensive data visualizations and analysis charts
- **Statistical Analysis**: Conducted detailed feature importance and performance analysis

### Technical Skills Demonstrated

- **Data Science**: Pandas, NumPy, data manipulation and analysis
- **Machine Learning**: Scikit-learn, Random Forest, hyperparameter tuning
- **Data Visualization**: Matplotlib, Seaborn, statistical plotting
- **Statistical Analysis**: Feature engineering, correlation analysis, performance metrics
- **Jupyter Notebooks**: Interactive data analysis and documentation
- **Data Preprocessing**: Cleaning, validation, and feature creation
- **Model Evaluation**: Cross-validation, confusion matrices, performance metrics

### Technologies Used

**Core**: Python 3.x, Pandas, NumPy, Scikit-learn
**Visualization**: Matplotlib, Seaborn
**Analysis**: Jupyter Notebooks, Statistical Analysis
**Data**: CSV processing, Data manipulation

## 📈 Future Enhancements

- [ ] Deep learning models (Neural Networks, LSTM)
- [ ] Additional features (economic, demographic, environmental)
- [ ] Real-time prediction updates
- [ ] Interactive web dashboard
- [ ] Integration with health policy databases
- [ ] Regional and sub-national analysis
- [ ] Time series forecasting models
- [ ] Ensemble methods for improved accuracy

## 👨‍💻 Author

**RD-Bhowmik**

- GitHub: [@RD-Bhowmik](https://github.com/RD-Bhowmik)
- Project Link: [Repository URL]

---

_This project demonstrates advanced data science skills, machine learning expertise, statistical analysis capabilities, and domain knowledge in public health - making it an excellent showcase of analytical and technical abilities for data science and public health positions._
