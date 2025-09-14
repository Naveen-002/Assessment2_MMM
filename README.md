# Assessment 2 – Marketing Mix Modeling with Mediation

## 📌 Project Overview
This project implements a **Marketing Mix Modeling (MMM)** approach with the mediation assumption that **Google spend acts as a mediator** between social media channels (Facebook, TikTok, Instagram, Snapchat) and Revenue.

The analysis is part of **Placement Assessment 2** and includes:
- Data preprocessing (trend, seasonality, log transformations)
- Mediation treatment (two-stage regression: Social → Google → Revenue)
- Modeling with ElasticNet and XGBoost
- Time-series cross-validation (no look-ahead)
- Diagnostics, residual analysis, and sensitivity tests (price & promotions)
- Insights and recommendations for marketing strategy

---

## ⚙️ Setup Instructions

### Option 1: Run in Google Colab (Recommended)
Click below to open the notebook directly in Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Naveen-002/Assessment2_MMM/blob/main/Assessment2_MMM.ipynb)

The dataset is automatically loaded from the repository using a GitHub raw link.  
No manual uploads required.

### Option 2: Run Locally
1. Clone the repo:
   ```bash
   git clone https://github.com/Naveen-002/Assessment2_MMM.git
   cd Assessment2_MMM
2. Install dependencies:
pip install -r requirements.txt
3. Launch Jupyter:
jupyter notebook Assessment2_MMM.ipynb
