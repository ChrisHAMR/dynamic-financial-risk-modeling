# Dynamic Financial Risk Modeling

This project investigates how financial risk evolves over time under nonstationarity, regime shifts, and extreme market events.  
The focus is on integrating volatility modeling, tail risk analysis, time–frequency methods, and Bayesian inference into a coherent statistical framework for dynamic portfolio decision-making.

Rather than optimizing performance metrics alone, the emphasis is on **understanding uncertainty**, **dependence structures**, and **regime-dependent risk behavior** in financial time series.

---

## Research Focus

- **Field:** Financial Risk, Time-Series Modeling, and Tail-Event Analysis  
- **Core Question:**  
  How do volatility, correlation, and dependence structures evolve across normal and extreme market regimes, and how can probabilistic models enable more robust portfolio decisions?

---

## Project Structure & Phases

### Phase 1 — Data Acquisition & Foundations
**Goal:** Build a clean, reproducible foundation for all downstream modeling.

**Key components:**
- Historical financial time-series retrieval (e.g., NASDAQ, S&P indices)
- Data cleaning and standardization
- Log-return construction
- Exploratory data analysis:
  - price and return visualization
  - rolling volatility and correlations
  - distributional characteristics (skewness, kurtosis)
- Initial risk indicators:
  - empirical volatility
  - drawdowns

**Deliverables:**
- `data/`
- `01_data_cleaning.ipynb`
- `02_initial_eda.ipynb`

---

### Phase 2 — Volatility Modeling (GARCH Family)
**Goal:** Quantify how volatility evolves over time under nonstationarity.

**Key components:**
- GARCH(1,1) modeling of log returns
- Comparison with asymmetric models (EGARCH / GJR-GARCH, optional)
- Interpretation of:
  - volatility persistence
  - leverage effects
  - high- and low-volatility regimes

**Deliverables:**
- `03_garch_modeling.ipynb`
- Conditional volatility and regime interpretation plots

---

### Phase 3 — Extreme Value Analysis (EVT)
**Goal:** Model tail behavior and quantify extreme market risk.

**Key components:**
- Peaks-Over-Threshold (POT) framework
- Generalized Pareto Distribution (GPD)
- Estimation of:
  - tail index
  - extreme quantiles
  - Value-at-Risk (VaR)
  - Expected Shortfall (ES)
- Comparison between normal and heavy-tailed assumptions

**Deliverables:**
- `04_evt_tail_risk.ipynb`
- Tail diagnostic plots (QQ tail, mean excess)
- Regime-aware tail risk discussion

---

### Phase 4 — Time–Frequency & Nonstationary Analysis
**Goal:** Capture how dependence and volatility evolve across time and frequency.

**Key components:**
- Time–frequency decomposition (STFT / wavelets / SLEX-style analysis)
- Evolving spectral density visualization
- Time-varying coherence between assets
- Identification of structural breaks and regime segmentation

**Deliverables:**
- `05_time_frequency_analysis.ipynb`
- Spectrograms and coherence heatmaps

---

### Phase 5 — Bayesian Modeling & Regime Learning
**Goal:** Introduce probabilistic modeling for uncertainty quantification and regime inference.

**Key components:**
- Bayesian AR / ARIMA models for return dynamics
- Bayesian volatility modeling (where applicable)
- Regime learning via:
  - Bayesian change-point detection
  - posterior inference
- Model comparison (WAIC / LOO)
- Posterior predictive checks

**Deliverables:**
- `06_bayesian_time_series.ipynb`
- Posterior summaries and regime segmentation results

---

### Phase 6 — Integrated Financial Risk Analysis
**Goal:** Synthesize all modeling components into a unified narrative.

**Key components:**
- Regime identification and labeling
- Volatility dynamics (GARCH-based)
- Tail risk behavior across regimes (EVT)
- Time–frequency dependence structure
- Bayesian uncertainty quantification
- Portfolio risk implications under regime shifts

**Deliverables:**
- `07_master_analysis.ipynb`
- Final synthesis figures and discussion

---

### Phase 7 — Final Polishing & Documentation
**Goal:** Present the project at a professional research standard.

**Key components:**
- Finalized README with methodological flow
- Clean project structure and documentation
- Citations and references
- Reproducibility and code clarity
- Exported PDF project summary

---

## Methodological Emphasis

- Time-series analysis under nonstationarity
- Volatility and tail risk modeling
- Time–frequency methods for evolving dependence
- Bayesian inference and uncertainty quantification
- Reproducible, workflow-based research

---

## Status

This project is developed as a progressive research pipeline.  
Individual phases may be updated iteratively as modeling depth increases.

---

## Disclaimer

This repository is intended for academic and research purposes only and does not constitute financial or investment advice.

**Status:** 🚧 Work in Progress
