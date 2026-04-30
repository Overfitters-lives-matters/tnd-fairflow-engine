# TND FairFlow Engine

### Real-Time Intrinsic Valuation and Liquidity Pressure Model for USD/TND

This project develops a two-layer econometric framework for valuing USD/TND:

- **Global FX Basket Model** (EUR/USD, GBP/USD, USD/JPY)
- **Local Liquidity Adjustment** (Kalman-filtered interbank spread)

## Key Features

- Log-return basket regression with HAC-robust inference
- Kalman filter calibrated via Maximum Likelihood (Q, R)
- Regime-aware liquidity modeling
- Real-time intrinsic value engine
- Rolling out-of-sample backtesting
- Diebold-Mariano forecast comparison
- Mincer-Zarnowitz efficiency test
- Regime-conditional performance analysis
- Kalman posterior confidence bands

## Output

The model produces: Intrinsic USD/TND = Baseline (global FX) + Local Liquidity Adjustment

## Purpose

Designed as a hybrid between:
- academic econometrics project
- FX desk valuation tool
- central bank-style monitoring framework

## Author

mariem abidi
