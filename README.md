# ESG-Screened Portfolio Optimizer

My project building applying university, python and financial modelling skills withe ESG knowledge to compare risk-adjusted returns between an unscreened stock universe and an ESG-screened universe with a sharpe-ratio diagram.

## Motivation

This project was built to apply portfolio theory and Python skills developed
through university and independent study to practical application. ESG integration is an
increasingly significant consideration in asset management, so this project
uses it as a test case to explore how a screening criterion affects
risk-adjusted portfolio performance in practice.

## Method

- Data: 5 years of daily prices (2020–2025), 9 large-cap US stocks across
  Energy, Tech and Consumer Staples, pulled via yfinance (Yahoo Finance).
- Calculated daily returns, annualised return/volatility, and the
  covariance matrix.
- ESG screen: excludes companies in the Energy sector as a proxy for
  fossil-fuel exposure.
- Used scipy.optimize to find the max-Sharpe-ratio portfolio and generate
  the efficient frontier for both portfolios.

## Finding

The full portfolio achieved a Sharpe ratio of 0.935, versus 0.904 for the
ESG-screened portfolio. A difference of 0.031 (3.32%), meaning the screened portfolio
required a slightly higher exposure to risk to achieve comparable returns over this period.

## Limitations

- The sector exclusion is a simplified ESG proxy, not a full ESG score.
- 9 stocks is a small sample size and the results are more indicative of the method used for the project,
  not a full-scale conclusion.
- Results are specific to this 2020–2025 sample period and would likely
  differ in other market conditions.

## A note on AI use

I used AI assistance to help understand and implement parts of this project
that went beyond my Python coursework.

## How to run

Open `Miguel Project.ipynb` in Google Colab and click run all.
