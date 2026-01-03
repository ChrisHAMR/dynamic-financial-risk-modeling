# 🧠 Dynamic Financial Risk Modeling  
**Volatility, Extreme Events, Time–Frequency Structure, and Bayesian Regime Learning**

---

## 📌 Project Overview

Financial market risk is **dynamic, nonstationary, and regime-dependent**.  
Periods of relative calm are punctuated by episodes of heightened volatility, structural breaks, and extreme losses—phenomena that are poorly captured by static or Gaussian risk models.

This project develops an **integrated statistical framework for dynamic financial risk modeling**, combining:

- Volatility modeling (GARCH family)
- Extreme Value Theory (EVT) for tail risk
- Time–frequency analysis for nonstationarity
- Bayesian inference for uncertainty quantification and regime learning

Rather than relying on a single modeling paradigm, the project demonstrates how **complementary statistical tools** jointly characterize different dimensions of market risk.

---

## 🎯 Research Motivation & Core Question

### Core Question
> **How does financial market risk evolve across regimes, temporal scales, and uncertainty layers, and what are the implications for risk-aware decision-making?**

### Key Themes
- Regime shifts and structural breaks  
- Heavy-tailed losses and extreme events  
- Persistent versus transient volatility dynamics  
- Multiscale (time–frequency) behavior  
- Bayesian uncertainty and probabilistic inference  

---

## 📊 Dataset

- **Asset**: S&P 500 Index  
- **Source**: stooq.pl (open-access financial data)  
- **Frequency**: Daily  
- **Time Span**: January 2000 – December 2025  
- **Primary Variable**: Log returns computed from closing prices  

All analyses are conducted on a **single, consistently processed dataset** to ensure reproducibility and internal coherence.

---

## 🧩 Project Structure & Phases

The project is organized as a **modular yet tightly integrated analytical pipeline**:

### ⭐ Phase 1 — Data Acquisition & Cleaning
- Raw data archival for reproducibility  
- Variable standardization and date processing  
- Construction of daily log returns  
- Clean, research-grade data pipeline  

📁 `01_data_cleaning.ipynb`

---

### ⭐ Phase 2 — Exploratory Data Analysis (EDA)
- Stylized facts of financial returns  
- Volatility clustering and distributional shape  
- Rolling volatility and empirical diagnostics  
- Motivation for dynamic and non-Gaussian models  

📁 `02_initial_eda.ipynb`

---

### ⭐ Phase 3 — Volatility Modeling (GARCH Family)
- GARCH(1,1), EGARCH, and GJR-GARCH models  
- Persistence, leverage effects, and regime intuition  
- Conditional volatility extraction  
- Endogenous volatility-based regime segmentation  

📁 `03_garch_modeling.ipynb`

---

### ⭐ Phase 4 — Extreme Value Theory (EVT)
- Peaks-Over-Threshold (POT) framework  
- Generalized Pareto Distribution (GPD)  
- Value-at-Risk (VaR) and Expected Shortfall (ES)  
- Comparison with Gaussian risk measures  

📁 `04_evt_tail_risk.ipynb`

---

### ⭐ Phase 5 — Time–Frequency & Nonstationary Analysis
- STFT-based time–frequency decomposition  
- Volatility dynamics across time and scale  
- SLEX-inspired interpretation of local stationarity  
- Compact numerical summaries for regime alignment  

📁 `05_time_frequency_analysis.ipynb`

---

### ⭐ Phase 6 — Bayesian Modeling & Regime Learning
- Bayesian AR(0) and AR(1) models  
- Posterior predictive checks  
- PSIS-LOO and WAIC model comparison  
- Bayesian change-point detection on volatility  
- Probabilistic regime identification  

📁 `06_bayesian_time_series.ipynb`

---

### ⭐ Phase 7 — Integration & Synthesis
- Unified, regime-aware interpretation  
- Volatility, tail risk, time–frequency, and Bayesian evidence combined  
- Implications for risk-sensitive decision-making  
- Research-style synthesis (no new models introduced)  

📁 `07_master_analysis.ipynb`

---

### ⭐ Phase 8 — Final Documentation
- Clean project structure  
- Reproducible outputs and figures  
- Exported numerical summaries for reporting  
- This README  

---

## 🔬 Methodological Philosophy

This project follows **modern statistical research principles**:

- **No single model is “true”** — models are evaluated based on explanatory power and predictive adequacy.  
- **Uncertainty is first-class**, not an afterthought.  
- **Regimes are descriptive**, not assumed latent truths.  
- **Interpretability and robustness** are prioritized over overfitting.  

Bayesian methods are used **where they add value**—for uncertainty quantification, model comparison, and regime learning—rather than as decorative complexity.

---

## 📈 Key Insights

- Volatility is **persistent and regime-dependent**, not smoothly varying.  
- Extreme losses exhibit **heavy-tailed behavior** that volatility alone cannot capture.  
- Market risk operates across **multiple temporal scales**, with crisis periods characterized by low-frequency dominance and broadband energy.  
- Regime transitions are **nonstationary** and best understood probabilistically rather than deterministically.  
- Risk-aware decision-making benefits from **regime awareness, tail sensitivity, and explicit uncertainty quantification**.  

---

## 🧠 Relevance to Graduate Research

This project aligns closely with research areas in:

- Financial econometrics  
- Time-series analysis  
- Nonstationary and multiscale modeling  
- Extreme value theory  
- Bayesian inference and model comparison  
- Risk management under regime uncertainty  

The full pipeline is designed to resemble a **mini research thesis**, suitable for MS/PhD-level review.

---

## 🔄 Reproducibility

- All analyses are conducted in Python.  
- Raw, processed, and results data are clearly separated.  
- No manual data manipulation occurs outside notebooks.  
- Figures and tables are generated programmatically.  
- Numerical summaries are exported as CSV files for reuse.  

---

## 🚀 Future Extensions

Natural extensions of this work include:

- Multivariate dependence modeling and joint tail risk across assets  
- Time-varying correlation, spectral coherence, and cross-market dependence  
- Regime-dependent portfolio decision frameworks under uncertainty  
- Online and sequential regime detection for real-time risk monitoring  
- Fully Bayesian volatility and regime-switching models  
- Adaptive time–frequency representations (e.g., SLEX, wavelet packets)
  
---

## 📎 Author Note

This project was developed as a **research-oriented portfolio** emphasizing methodological rigor, interpretability, and uncertainty-aware inference.  
It is intentionally designed to bridge applied financial modeling and modern statistical research.

---

**Status:** ✔ Complete — Research-grade dynamic financial risk modeling pipeline
