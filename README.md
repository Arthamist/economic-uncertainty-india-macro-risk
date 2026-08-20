# Economic Uncertainty in India: Macroeconomic Risk Analysis

## Project Overview

This research project develops a composite measure of economic uncertainty in India and examines its time-varying relationship with macroeconomic and financial-market variables during 2016–2022.

The analysis combines **Principal Component Analysis (PCA)** to construct a Composite Uncertainty Index with a **Bayesian Time-Varying Parameter VAR (TVP-VAR)** framework and time-varying impulse response analysis.

### Research Question

**How does economic uncertainty affect India's economy and financial markets, and how does the impact change over time?**

## Analytical Framework

```text
Economic Policy Uncertainty (EPU)
India VIX
Inflation Volatility
          |
          v
        PCA
          |
          v
Composite Uncertainty Index
          |
          v
Bayesian TVP-VAR
          |
          v
Time-Varying Impulse Responses
          |
          v
Macroeconomic & Financial Risk Analysis
```

## Data & Variables

**Period:** 2016–2022  
**Frequency:** Monthly Indian data

### Uncertainty Measures
- Economic Policy Uncertainty (EPU)
- India VIX
- Inflation volatility estimated using GARCH-based conditional variance

### Macroeconomic Variables
- GDP
- Unemployment rate
- Merchandise exports

### Financial-Market Variables
- Exchange rate (INR/USD)
- 182-day Treasury Bill yield
- NIFTY
- SENSEX

### Sources
- Economic Policy Uncertainty
- NSE India
- Ministry of Statistics & Programme Implementation (MoSPI)
- Ministry of Commerce
- Financial Benchmarks India Pvt. Ltd. (FBIL)
- CMIE
- BSE India

## Methodology

1. **Data preparation** — monthly data collection, missing-value handling, alignment and transformations where required.
2. **Uncertainty measurement** — EPU, India VIX and inflation volatility.
3. **Composite Uncertainty Index** — standardisation followed by PCA; the first principal component is used as the composite index.
4. **Bayesian TVP-VAR** — estimation using Markov Chain Monte Carlo (MCMC).
5. **Dynamic analysis** — time-varying impulse responses and forecast error variance decomposition to examine macro-financial responses.

## Key Findings

### Economic Activity
- Economic uncertainty was highly time-varying, with the strongest spike occurring around 2020.
- GDP and exports showed adverse responses around major uncertainty episodes.
- Unemployment displayed a prolonged increase following major uncertainty shocks.
- Treasury Bill yields generally moved inversely with the uncertainty index.

### Financial Markets
- NIFTY and SENSEX showed negative short-run responses following uncertainty shocks.
- Financial-market responses varied across periods and showed evidence of adjustment and recovery over longer horizons.
- Exchange-rate responses indicated stronger depreciation pressure during periods of elevated uncertainty.

### Time-Varying Effects
The estimated responses were not constant over time. The COVID-19 period showed the strongest and most widespread adverse responses, while several post-COVID responses became weaker or normalised.

## Policy & Risk Interpretation

The findings suggest that economic uncertainty can act as an important transmission channel between major shocks and macroeconomic and financial conditions.

The analysis highlights the relevance of:
- clear and predictable policy communication,
- external-sector resilience,
- support for economic activity during uncertainty shocks, and
- financial-market resilience and liquidity.

## Technical Skills Demonstrated

**R · Econometrics · PCA · Bayesian Time Series · TVP-VAR · MCMC · GARCH · Impulse Response Analysis · Macroeconomic Risk Analysis**

## Project Presentation

The complete presentation is included in this repository:

**[View the project presentation](Economic_Uncertainty_India_Macro_Risk_Analysis.pdf)**

## Note

This repository is intentionally presentation-focused. The uploaded artifact communicates the research question, data, methodology, empirical results, interpretation, and policy implications without publishing the underlying research code or dataset.
