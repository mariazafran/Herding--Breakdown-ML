
# Machine Learning Analysis of Herding Breakdown in Financial Markets

## Short Introduction

This project investigates **herding behaviour in financial markets** and introduces a novel extension using **machine learning to detect and explain the breakdown of herding**.

Traditional studies focus on identifying the presence of herding.  
This research shifts the focus to a more important question:

> **When does herding break down?**

---

## Motivation

Herding behaviour implies that investors move collectively.  
However, during periods of **high market uncertainty and volatility**, this collective behaviour may weaken or disappear.

This project explores whether:

- Herding persists under volatile conditions  
- Or markets become **fragmented, with investors acting independently**

---

##  Key Contribution

This study introduces a **data-driven framework** to analyse herding breakdown:

### Novel Elements

- Construction of a **herding breakdown indicator**
- Application of **machine learning (Random Forest)** to estimate breakdown probability
- Use of **nonlinear visualisation (LOWESS smoothing)**
- Focus on **dispersion and breakdown rather than traditional herding detection**

---

## Key Findings

- Herding behaviour is **not observed during high volatility**
- Market dispersion increases as volatility rises
- The probability of herding breakdown increases **nonlinearly with volatility**
- Investor behaviour becomes increasingly **divergent under uncertainty**

>  **Main Insight:**  
> Higher volatility leads to a systematic breakdown of collective market behaviour.

---

## View Notebook

🔗 **Run in Google Colab (interactive):**  
https://colab.research.google.com/github/mariazafran/Herding--Breakdown-ML/blob/main/Herding_Breakdown_ML.ipynb  

 **View notebook (recommended):**  
https://nbviewer.org/github/mariazafran/Herding--Breakdown-ML/blob/main/Herding_Breakdown_ML.ipynb

---

##  Methodology

### 1. Data Preparation
- FTSE stock data (via `yfinance`)
- Return calculation and cleaning
- Construction of market return (Rm)

---

### 2. Herding Measurement
- Cross-sectional Absolute Deviation (CSAD)
- Used as proxy for investor coordination

---

### 3. Econometric Analysis
- OLS regression models
- Volatility modelling (GARCH)
- Testing for presence/absence of herding

---

### 4. Machine Learning Extension

- Random Forest classification model  
- Creation of **herding breakdown variable**  
- Estimation of **breakdown probability**  
- Rolling smoothing to remove noise  
- Nonlinear visualisation using LOWESS  

---

##  Key Visual Insights

### 🔹 Smoothed Breakdown Probability
- Shows that breakdown behaviour is **dynamic and time-varying**
- Market behaviour evolves rather than remaining stable  

---

###  Volatility vs Breakdown Probability
- Reveals a **strong nonlinear relationship**
- Breakdown probability increases sharply at higher volatility levels  

---

## Interpretation

The results suggest that:

- Markets do not become more coordinated during stress  
- Investors behave **independently and heterogeneously**  
- This leads to increased dispersion and **breakdown of herding**  

---

## Practical Implications

This framework is useful for:

- Risk management  
- Identifying **market instability**  
- Understanding investor behaviour under uncertainty  
- Supporting portfolio diversification strategies  

---

##  Note on Notebook Viewing

GitHub may not display Jupyter notebooks correctly due to rendering limitations.

 Please use the links above for full access:
- Google Colab (interactive)
- nbviewer (full display)

---

##  Author

Maria Bibi  
Research (Economics & Finance)

---

## Citation

Bibi, M. (2026).  
*Machine Learning Analysis of Herding Breakdown in Financial Markets*.  
Available at: https://github.com/mariazafran/Herding-Breakdown-ML
