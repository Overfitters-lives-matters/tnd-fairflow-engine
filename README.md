# TND FairFlow Engine
### Real-Time Intrinsic Valuation and Liquidity Pressure Model for USD/TND

---

## Overview

The **TND FairFlow Engine** is a two-layer econometric framework designed to estimate the intrinsic value of USD/TND by combining:

- **Global FX fundamentals** (EUR/USD, GBP/USD, USD/JPY)
- **Local Tunisian liquidity conditions** (interbank vs fixing spread)

Unlike the official fixing, the model produces a **market-consistent fair value** that reflects both international dynamics and domestic frictions.

---

## Model Architecture

\[
Intrinsic_{t} = Baseline_{t} + Adjustment_{t}
\]

### 1. Global Basket Baseline
- Log-return regression
- HAC (Newey-West) robust inference
- Rolling and static specifications

### 2. Liquidity Adjustment
- Kalman filter (MLE-calibrated Q, R)
- Regime-aware spread dynamics
- AR + state-space hybrid modeling

---

## Key Contributions

- ✔ Intrinsic USD/TND valuation beyond official fixing  
- ✔ Maximum Likelihood Kalman calibration  
- ✔ Diebold-Mariano statistical validation  
- ✔ Mincer-Zarnowitz forecast efficiency testing  
- ✔ Regime-conditional performance analysis  
- ✔ Real-time valuation architecture  

---

## Results

The FairFlow model improves forecast accuracy relative to the fixing-only benchmark and provides economically meaningful decomposition between:

- global FX-driven movements  
- local liquidity-driven distortions  

---

## Use Cases

- Treasury FX valuation  
- Central bank monitoring  
- Market stress diagnostics  
- Risk management  

---


## Tech Stack

- Python  
- pandas / numpy  
- statsmodels  
- scipy  
- matplotlib  

---

## Author

mariem abidi
