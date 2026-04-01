# Value at Risk (VaR) Model in Python

## Project Description
This project implements a Value at Risk (VaR) model to measure financial risk using historical market data.
The objective is to estimate the maximum expected loss of an asset over a given time horizon at a specified confidence level.
---

## What does this project do?
- Quantifies financial risk using the Value at Risk (VaR) metric  
- Estimates the potential loss of an asset under normal market conditions  
- Compares different VaR methodologies  
- Provides visual and statistical analysis of asset returns  
---

## Data Used
- Source: Yahoo Finance  
- Asset: Apple Inc. (AAPL) *(configurable to any stock, index, or commodity)*  
- Frequency: Daily adjusted closing prices  
- Time period: Configurable (default: 2015–2025)  
---

## Methodology
The project implements two approaches for VaR estimation:

### 1. Historical VaR
- Based on the empirical distribution of returns  
- No assumptions about the underlying distribution  
- Calculated using the lower percentile of returns  

### 2. Parametric VaR (Normal)
- Assumes returns follow a normal distribution  
- Uses mean (μ) and standard deviation (σ)  
- Applies the Z-score corresponding to the confidence level  
---

## Process
1. Download financial data  
2. Compute logarithmic returns  
3. Calculate descriptive statistics
4. Estimate VaR (Historical & Parametric)  
5. Visualize results  
---

## Main Result
The model estimates the maximum expected daily loss of the asset at a given confidence level.

Example interpretation:
> At a 95% confidence level, the model indicates that the maximum expected daily loss will not exceed a specific percentage under normal market conditions.
---

## Visualizations
- Time series of returns  
- Histogram of returns  
- VaR thresholds (Historical vs Parametric)  
---

## How to Run

1. Open the notebook in Google Colab  
2. Install dependencies:
```python
!pip install yfinance
