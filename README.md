# The Drivers of Venture Capital Performance 📈

Capstone Project – Duke University (Team 58)  
By Jamie Fobel, Jessica Liang, Lydia Luo, David Chang, and Moshu Huang  

## 📖 Project Overview

This project investigates the drivers of **Venture Capital (VC) fund performance since 2000**, using data from **Preqin** and other sources.  
Our objective is **explanatory modeling** – not just predicting outcomes, but explaining why funds succeed or fail based on structural, operational, and macroeconomic factors.

By uncovering the causal links between fund attributes and performance, our findings provide guidance for **General Partners (GPs)** and **Limited Partners (LPs)** to optimize allocation strategies, benchmark new opportunities, and understand empirically validated drivers of performance.

## ⚙️ Methodology

- **Exploratory Data Analysis (EDA):** examining fund- and firm-level characteristics  
- **Explanatory Modeling:** focusing on *why* funds succeed rather than ex ante prediction  
- **Cross-Validation:** applied to guard against overfitting  
- **Unsupervised Learning:** PCA for dimensionality reduction, K-Means clustering for fund archetypes  
- **Supervised Learning:** Random Forest and XGBoost to evaluate factor importance on Net IRR  

Key distinction:  
- Predictive modeling emphasizes out-of-sample accuracy.  
- Our **explanatory modeling** emphasizes causal interpretation, using in-sample performance while ensuring robustness.

## 📚 Literature Framework

Past studies highlight several fund-level performance metrics:  
- **Internal Rate of Return (IRR):** annualized profitability at fund level  
- **Total Value to Paid-In (TVPI):** capital efficiency ratio  
- **Public Market Equivalent (PME):** benchmark against public equity indices  

These metrics are often correlated and must be interpreted jointly.  
We build on prior research (Kaplan & Schoar, 2005; Harris et al., 2014) and extend analysis with modern data science methods.

## 📊 Key Findings

- **Timing dominates:** funds launched in favorable macro cycles outperform peers.  
- **Pacing matters:** disciplined capital deployment and quick distributions enhance returns.  
- **Fund structure counts:** mid-sized, agile funds outperform mega-funds.  
- **Active engagement:** dynamic post-investment management (picking winners) is linked to higher IRR.  

Together, these findings show that VC success reflects the **interaction of external conditions, internal execution, and fund design choices**.

## 🛠 Tech Stack

- Python (pandas, numpy, scikit-learn, xgboost)  
- Tableau (dashboards for fund-level analysis)  
- Jupyter Notebook  

## 📂 Repository Structure

```text
vc-performance-drivers/
├── data/                       # Example / simulated data (anonymized)
├── notebooks/                  # Jupyter notebooks for EDA and modeling
├── models/                      # Saved ML models and results
├── results/                     # Figures and summary outputs
├── requirements.txt
└── README.md
