# 📈 Portfolio Beta & CAPM Calculator

## Overview

This project calculates the **Portfolio Beta** and **Expected Return using the Capital Asset Pricing Model (CAPM)** for a portfolio of stocks and ETFs.

The tool combines portfolio holdings, asset betas, and market assumptions to estimate the portfolio's overall market risk and expected return.

This project was built as part of my learning journey in portfolio management, investment analysis, and quantitative finance.

---

## Features

* Calculate individual asset weights
* Calculate weighted portfolio beta
* Estimate portfolio expected return using CAPM
* Support stocks, ETFs, and cash positions
* Easy-to-use Excel-based implementation
* Flexible inputs for portfolio holdings and market assumptions

---

## Finance Concepts Used

## Portfolio Weight

The proportion of total portfolio value invested in each asset.

$$
Weight_i = \frac{Investment_i}{Total\ Portfolio\ Value}
$$

## Beta

Beta measures how sensitive an asset is to movements in the overall market.

- Beta = 1.0 → Moves with the market
- Beta > 1.0 → More volatile than the market
- Beta < 1.0 → Less volatile than the market

## Portfolio Beta

Portfolio beta is the weighted average beta of all portfolio holdings.

$$
Portfolio\ Beta = \sum (Weight_i \times Beta_i)
$$

## CAPM

The Capital Asset Pricing Model estimates the expected return of a portfolio based on its market risk.

$$
Expected\ Return = R_f + \beta_p (R_m - R_f)
$$

Where:

- $R_f$ = Risk-Free Rate
- $\beta_p$ = Portfolio Beta
- $R_m$ = Expected Market Return
  
## Example Inputs

| Asset  | Beta |
| ------ | ---- |
| RY.TO  | 0.94 |
| TD.TO  | 0.88 |
| BMO.TO | 1.16 |
| BN.TO  | 1.84 |
| CM.TO  | 1.28 |

Additional holdings can be added as needed.

---

## Excel Implementation

### Portfolio Beta

```excel
=SUMPRODUCT(Weight_Range,Beta_Range)
```

### Market Risk Premium

```excel
=Expected_Market_Return - Risk_Free_Rate
```

### CAPM Expected Return

```excel
=Risk_Free_Rate + Portfolio_Beta*(Market_Return-Risk_Free_Rate)
```

## Technologies Used

* Excel
* Python
* Pandas
* Yahoo Finance (yfinance)
* GitHub

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Portfolio Risk Measurement
* CAPM Framework
* Beta Analysis
* Investment Analytics
* Financial Modeling
* Python for Financial Data Analysis
* Excel-based Financial Tools

---

## Disclaimer

This project is intended for educational and informational purposes only.

Nothing contained in this repository should be considered financial, investment, tax, or legal advice. The calculations and examples are provided solely for learning and demonstration purposes. Always conduct your own research and consult a qualified financial professional before making investment decisions.

---

## Author

**Dr. Sohom Mandal, Ph.D., P.Eng.**

Data Scientist | AI Professional | Finance Enthusiast

GitHub: https://github.com/sohomiitb

LinkedIn: https://www.linkedin.com/in/sohomiitb
