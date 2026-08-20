# Economic Uncertainty in India: Macroeconomic Risk Analysis

> **Measuring the time-varying impact of economic uncertainty on India's economy and financial markets**

**Master's Dissertation | Economics | R • Econometrics • Bayesian Time Series**

---

## 1. Project Overview

Economic uncertainty can affect economic activity, employment, financial markets, and investor behaviour. This research develops a composite measure of economic uncertainty for India and examines how its effects vary across different periods, with particular focus on the COVID-19 episode.

The study combines three dimensions of uncertainty:

- **Economic Policy Uncertainty (EPU)** — policy-related uncertainty captured through newspaper coverage
- **India VIX** — expected near-term equity-market volatility
- **Inflation volatility** — conditional volatility estimated using a GARCH model

These measures are combined using **Principal Component Analysis (PCA)** to construct a Composite Uncertainty Index. The index is then incorporated into a **Bayesian Time-Varying Parameter VAR (TVP-VAR)** framework to examine the dynamic response of macroeconomic and financial variables to uncertainty shocks.

The analysis covers **monthly Indian data from 2016–2022**, allowing comparison across pre-COVID, COVID, and post-COVID periods.

---

## 2. Research Questions

The study addresses three questions:

1. How does economic uncertainty affect key macroeconomic variables in India?
2. How does economic uncertainty affect Indian financial markets?
3. How do these relationships change across pre-COVID, COVID, and post-COVID periods?

---

## 3. Analytical Framework

```text
Economic Policy Uncertainty (EPU)
              +
          India VIX
              +
     Inflation Volatility
              │
              ▼
             PCA
              │
              ▼
  Composite Uncertainty Index
              │
              ▼
     Bayesian TVP-VAR
              │
              ▼
 Time-Varying Impulse Responses
              │
              ▼
 Macroeconomic & Financial-Market
          Risk Analysis
```

---

## 4. Data

**Period:** 2016–2022  
**Frequency:** Monthly

### Uncertainty Measures

| Measure | Role |
|---|---|
| Economic Policy Uncertainty (EPU) | Policy-related uncertainty |
| India VIX | Expected market volatility |
| Inflation volatility | Conditional inflation uncertainty estimated using GARCH |

### Response Variables

**Macroeconomic**
- GDP
- Unemployment rate
- Exports

**Financial**
- INR/USD exchange rate
- 182-day Treasury Bill yield
- NIFTY returns
- SENSEX returns

### Data Sources

- Economic Policy Uncertainty — PolicyUncertainty.com
- India VIX — NSE India
- Inflation & GDP — Ministry of Statistics and Programme Implementation (MoSPI)
- Exports — Ministry of Commerce
- Unemployment — CMIE
- Exchange rate & T-Bill yield — Financial Benchmarks India Pvt. Ltd. (FBIL)
- NIFTY — Yahoo Finance
- SENSEX — BSE India

### Data Preparation

The dissertation uses monthly observations from 2016–2022. GDP was originally available at quarterly frequency and was converted to monthly frequency using the **Denton–Cholette method**, with the **Index of Industrial Production (IIP)** used as the benchmark.

Stationarity was assessed using the **Augmented Dickey-Fuller (ADF) test**. Non-stationary variables were transformed through first differencing before the TVP-VAR analysis.

---

## 5. Methodology

### Step 1 — Inflation Volatility

Inflation was transformed into a stationary series and a **GARCH model** was used to estimate its conditional variance. The resulting volatility measure forms one component of the uncertainty index.

### Step 2 — Composite Uncertainty Index

The three uncertainty measures were standardised and combined using **Principal Component Analysis**.

The **first principal component (PC1)** was selected as the Composite Uncertainty Index because it captures the largest share of common variation across the underlying uncertainty measures.

### Step 3 — Bayesian TVP-VAR

A **Time-Varying Parameter Vector Autoregression (TVP-VAR)** model was estimated using Bayesian inference and **Markov Chain Monte Carlo (MCMC)** methods.

Unlike a conventional VAR, the TVP-VAR allows the relationships between uncertainty and the macroeconomic/financial variables to evolve over time.

### Step 4 — Dynamic Response Analysis

Impulse response analysis was used to examine how the selected variables respond to an identified uncertainty shock over:

- **6-month horizons**
- **12-month horizons**

Responses were examined across representative periods including pre-COVID, COVID, and post-COVID conditions.

---

## 6. Key Findings

### Economic Activity

The Composite Uncertainty Index shows pronounced spikes during major uncertainty episodes, with the **largest spike occurring around April 2020** during the COVID-19 lockdown period.

The analysis indicates that higher uncertainty was associated with weaker economic outcomes:

- **GDP:** negative response, particularly during the COVID period
- **Exports:** negative and relatively persistent response around major uncertainty episodes
- **Unemployment:** upward response following major uncertainty shocks
- **T-Bill yields:** generally showed an inverse relationship with the uncertainty index, with the response varying across periods

### Financial Markets

The financial-market variables also displayed time-varying responses:

- **NIFTY:** negative short-run response following uncertainty shocks
- **SENSEX:** negative response during high-uncertainty periods, with recovery at longer horizons
- **Exchange rate:** evidence of depreciation pressure during periods of elevated uncertainty
- **T-Bill yield:** generally moved inversely with uncertainty, although major episodes produced different short-run dynamics

### COVID-19 and Time Variation

The central finding is that the effects of uncertainty **were not constant over time**.

The COVID-19 period produced the strongest and most widespread responses across the variables examined. Several responses became weaker or moved closer to baseline during the post-COVID period, while renewed uncertainty in 2022 generated different responses across variables.

---

## 7. Main Insight

A key conclusion of the research is:

> **Economic uncertainty acts as an important transmission channel through which major shocks can affect India's macroeconomic performance and financial-market conditions, with the magnitude and persistence of these effects changing over time.**

The study therefore goes beyond measuring whether uncertainty is high or low; it examines **how the economic consequences of an uncertainty shock evolve across different periods.**

---

## 8. Risk & Policy Interpretation

The findings have implications for macroeconomic and financial-risk monitoring.

The research highlights the importance of:

- **Policy clarity:** predictable policy communication can help reduce uncertainty-driven disruption.
- **External-sector resilience:** elevated uncertainty can create pressure on exchange rates and exports.
- **Economic stabilisation:** timely fiscal and public-investment measures can help cushion economic activity and employment during major shocks.
- **Financial-market resilience:** credible monetary policy communication and adequate market liquidity can help manage uncertainty-related volatility.

---

## 9. What This Project Demonstrates

**Econometrics**
- PCA-based index construction
- ADF stationarity testing
- GARCH volatility modelling
- Bayesian TVP-VAR
- MCMC estimation
- Impulse response analysis
- Time-varying macroeconomic analysis

**Economic & Risk Analysis**
- Macroeconomic risk measurement
- Financial-market risk analysis
- Uncertainty transmission
- Shock-response analysis
- Period-based comparative analysis
- Policy interpretation

**Tools**
- R
- Econometric and statistical modelling

---

## 10. Project Presentation

The complete research presentation is available in this repository:

**[View the presentation](Economic_Uncertainty_India_Macro_Risk_Analysis.pdf)**

The presentation summarises the research question, data, methodology, uncertainty-index construction, impulse-response results, overall findings, and policy implications.

---

## 11. Project Scope

This repository is intentionally **presentation-focused**. It contains the final research presentation rather than the underlying dataset or source code.

The project was originally completed as a **Master's dissertation in Economics** and has been presented here as a research and analytics portfolio project.

---

## Author

**Aditi Kushwaha**

**M.Sc. Economics | Applied Analytics | Econometrics | Risk & Financial Analysis**
