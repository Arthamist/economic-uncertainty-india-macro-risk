# Economic Uncertainty in India: Macroeconomic Risk Analysis

> **Measuring the time-varying impact of economic uncertainty on India's economy and financial markets**

**Master's Dissertation | Economics | R • Econometrics • Bayesian Time Series**

---

## Project at a Glance

Economic uncertainty can influence economic activity, employment, exchange rates, and financial-market conditions. This research develops a **Composite Economic Uncertainty Index for India** and examines how uncertainty shocks transmit through the economy and financial markets over time.

The study combines:

**EPU + India VIX + Inflation Volatility**  
↓  
**Principal Component Analysis (PCA)**  
↓  
**Composite Uncertainty Index**  
↓  
**Bayesian Time-Varying Parameter VAR (TVP-VAR)**  
↓  
**Time-Varying Impulse Response Analysis**  
↓  
**Macroeconomic & Financial Risk Insights**

The analysis uses **monthly Indian data from 2016–2022**, allowing the effects of uncertainty to be examined across **pre-COVID, COVID, and post-COVID periods**.

---

## Research Questions

The study addresses three questions:

1. **How does economic uncertainty affect key macroeconomic variables in India?**
2. **How does economic uncertainty affect Indian financial markets?**
3. **How do these relationships change across pre-COVID, COVID, and post-COVID periods?**

---

## Key Findings

### Economic Activity

The Composite Uncertainty Index shows pronounced increases during major uncertainty episodes, with the largest spike occurring around **April 2020** during the COVID-19 lockdown period.

The estimated responses indicate:

- **GDP:** negative response, particularly during the COVID period
- **Exports:** negative and relatively persistent response around major uncertainty episodes
- **Unemployment:** upward response following major uncertainty shocks

### Financial Markets

The financial-market variables also exhibit time-varying responses:

- **NIFTY:** negative short-run response following uncertainty shocks
- **SENSEX:** negative response during high-uncertainty periods, followed by recovery at longer horizons
- **Exchange rate:** evidence of depreciation pressure during periods of elevated uncertainty
- **T-Bill yields:** generally moved inversely with uncertainty, although responses varied across periods

### Time-Varying Effects

The central finding is that the effects of uncertainty **are not constant over time**.

The COVID-19 period produced the strongest and most widespread responses across the variables examined. Several responses became weaker or moved closer to baseline during the post-COVID period, while renewed uncertainty in 2022 produced different responses across variables.

---

## Data

**Period:** 2016–2022  
**Frequency:** Monthly

### Uncertainty Measures

| Measure | Role |
|---|---|
| Economic Policy Uncertainty (EPU) | Policy-related uncertainty |
| India VIX | Expected near-term equity-market volatility |
| Inflation volatility | Conditional inflation uncertainty estimated using GARCH |

### Macroeconomic Variables

- GDP
- Unemployment rate
- Exports

### Financial Variables

- INR/USD exchange rate
- 182-day Treasury Bill yield
- NIFTY returns
- SENSEX returns

### Data Sources

| Variable / Measure | Source |
|---|---|
| Economic Policy Uncertainty | PolicyUncertainty.com |
| India VIX | NSE India |
| Inflation & GDP | Ministry of Statistics and Programme Implementation (MoSPI) |
| Exports | Ministry of Commerce |
| Unemployment | CMIE |
| Exchange rate & T-Bill yield | Financial Benchmarks India Pvt. Ltd. (FBIL) |
| NIFTY | Yahoo Finance |
| SENSEX | BSE India |

---

## Data Preparation

The analysis uses monthly observations from 2016–2022.

GDP was originally available at quarterly frequency and was converted to monthly frequency using the **Denton–Cholette method**, with the **Index of Industrial Production (IIP)** used as the benchmark.

Stationarity was assessed using the **Augmented Dickey-Fuller (ADF) test**. Non-stationary variables were transformed through first differencing before the TVP-VAR analysis.

---

## Methodology

### 1. Inflation Volatility

Inflation was transformed into a stationary series and a **GARCH model** was used to estimate its conditional variance.

The resulting volatility measure was used as one component of the Composite Uncertainty Index.

### 2. Composite Uncertainty Index

The three uncertainty measures were standardised and combined using **Principal Component Analysis (PCA)**.

The **first principal component (PC1)** was selected as the Composite Uncertainty Index because it captures the largest share of common variation across the underlying uncertainty measures.

### 3. Bayesian TVP-VAR

A **Time-Varying Parameter Vector Autoregression (TVP-VAR)** model was estimated using Bayesian inference and **Markov Chain Monte Carlo (MCMC)** methods.

The TVP-VAR framework allows relationships between uncertainty and the macroeconomic and financial variables to evolve over time rather than remaining fixed throughout the sample.

### 4. Dynamic Response Analysis

Impulse response analysis was used to examine how the selected variables respond to an **identified uncertainty shock** over:

- **6-month horizons**
- **12-month horizons**

Responses were examined across representative pre-COVID, COVID, and post-COVID periods.

---

## Analytical Framework

```text
                  UNCERTAINTY MEASURES
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
         EPU         India VIX    Inflation Volatility
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                       PCA
                         │
                         ▼
             COMPOSITE UNCERTAINTY INDEX
                         │
                         ▼
                 BAYESIAN TVP-VAR
                         │
                         ▼
             TIME-VARYING IMPULSE
                  RESPONSES
                         │
                         ▼
             MACROECONOMIC & FINANCIAL
                    RISK ANALYSIS
```

---

## Risk & Economic Interpretation

The results indicate that economic uncertainty is an important transmission channel through which major shocks are associated with changes in India's macroeconomic and financial-market conditions.

The findings have implications for:

- **Policy clarity** — predictable policy communication can help reduce uncertainty-driven disruption.
- **External-sector resilience** — elevated uncertainty can create pressure on exchange rates and exports.
- **Economic stabilisation** — timely fiscal and public-investment measures can help cushion economic activity and employment during major shocks.
- **Financial-market resilience** — credible monetary-policy communication and adequate market liquidity can help manage uncertainty-related volatility.

The analysis therefore focuses not only on whether uncertainty is high or low, but also on **how the economic consequences of an uncertainty shock evolve across different periods**.

---

## Methods & Quantitative Skills

### Econometrics & Quantitative Methods

- Principal Component Analysis (PCA)
- ADF stationarity testing
- GARCH volatility modelling
- Bayesian Time-Varying Parameter VAR (TVP-VAR)
- Markov Chain Monte Carlo (MCMC) estimation
- Impulse response analysis
- Time-varying macroeconomic analysis

### Risk & Economic Analysis

- Macroeconomic risk measurement
- Financial-market risk analysis
- Economic uncertainty measurement
- Uncertainty transmission analysis
- Shock-response analysis
- Pre-COVID, COVID, and post-COVID comparison
- Policy and risk interpretation

### Tool

**R**

---

## Project Presentation

The complete research presentation is available below:

**[View the Economic Uncertainty & Macroeconomic Risk Analysis presentation](Economic_Uncertainty_India_Macro_Risk_Analysis.pdf)**

The presentation covers:

- Research questions
- Data and variables
- Composite Uncertainty Index
- Methodology
- Dynamic impulse responses
- Key findings
- Risk and policy interpretation

---

## Project Scope

This repository is intentionally **presentation-focused**.

It contains the final research presentation rather than the underlying research code or dataset. The project was originally completed as a **Master's dissertation in Economics** and is presented here as a research and analytics portfolio project.

---

## Author

**Aditi Kushwaha**
