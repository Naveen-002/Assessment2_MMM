# Assessment 2: MMM Modeling with Mediation Assumption

## Overview
This repository contains a comprehensive Media Mix Modeling (MMM) analysis that treats Google spend as a mediator between social/display channels and Revenue. The analysis follows industry best practices for causal inference, time-series validation, and business impact assessment.

## Key Features
- **Causal Framing**: Two-stage mediation analysis with Google as mediator
- **Technical Rigor**: Time-series cross-validation, robust preprocessing
- **Model Comparison**: ElasticNet vs XGBoost with performance evaluation
- **Business Insights**: Price elasticity, channel contributions, recommendations

## Repository Structure
```
Assessment2_MMM/
├── README.md                    # This file
├── requirements.txt             # Python dependencies
├── Assessment2_MMM.ipynb       # Main analysis notebook
└── environment.yml             # Conda environment (optional)
```

## Environment Setup

### Option 1: Using pip
```bash
# Clone the repository
git clone <repository-url>
cd Assessment2_MMM

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook Assessment2_MMM.ipynb
```

### Option 2: Using conda
```bash
# Clone the repository
git clone <repository-url>
cd Assessment2_MMM

# Create conda environment
conda env create -f environment.yml

# Activate environment
conda activate mmm-analysis

# Launch Jupyter
jupyter notebook Assessment2_MMM.ipynb
```

## Data Requirements
- Place your dataset as `Assessment 2 - MMM Weekly.csv` in the same directory
- Ensure the dataset contains the required columns: week, revenue, facebook_spend, tiktok_spend, instagram_spend, snapchat_spend, google_spend, emails_send, sms_send, average_price, promotions, followers

## Analysis Structure

### 1. Data Preparation
- Weekly seasonality handling
- Trend analysis
- Zero-spend period management
- Log transformations

### 2. Causal Framing
- Google as mediator assumption
- Two-stage modeling approach
- Mediation analysis

### 3. Modeling
- ElasticNet with regularization
- XGBoost for comparison
- Time-series cross-validation

### 4. Diagnostics
- Out-of-sample performance
- Residual analysis
- Sensitivity testing

### 5. Business Insights
- Price elasticity analysis
- Channel contribution ranking
- Strategic recommendations

## Key Results
- **Mediation Model R²**: Shows how well social channels predict Google spend
- **Revenue Model R²**: ElasticNet and XGBoost performance comparison
- **Price Sensitivity**: Impact of price changes on revenue
- **Channel ROI**: Ranking of marketing channels by effectiveness

## Reproducibility
- All random seeds set to 42
- Deterministic data preprocessing
- Time-series aware cross-validation
- Consistent feature engineering

## Dependencies
See `requirements.txt` for complete list of Python packages.

## Usage
1. Set up environment using instructions above
2. Place dataset in repository directory
3. Run all cells in `Assessment2_MMM.ipynb`
4. Review results and insights

## Contact
For questions about this analysis, please refer to the detailed methodology sections in the notebook.

---
*Analysis completed: 2024*
