# Star Cement Limited — DCF Valuation & Equity Research Model

A full equity research build-out on **Star Cement Limited** (NSE: `STARCEMENT` | BSE: `540575` | ISIN: `INE460H01021`), covering a 3-statement forecast, DCF valuation, peer comparables, and a daily market-tracking report.

> **Disclaimer:** This repository is prepared solely for educational and academic purposes as part of a financial modelling exercise. It does not constitute investment advice. All projections and valuations are the output of a modelling exercise built on publicly available data (company filings, Yahoo Finance, industry reports) and should not be relied upon for investment decisions. Consult a SEBI-registered investment advisor before acting on any information here.

---

## 📁 Repository Structure

```
star-cement-valuation/
│
├── Annual Reports/                          # Source filings used to build the model
│
├── Management report -2024-25.pdf           # FY2024-25 management discussion & analysis
├── Star-Cement_IP_Q4_FY26_Final.pdf         # Q4 FY26 Investor Presentation
│
├── Star Cements.xlsx                        # Core financial model (DCF, comps, WACC, ratios)
├── Star_Cement_Weekly_Returns.xlsx          # Weekly stock return tracking sheet
│
├── Star_Cement_Daily_Analysis_Report.pdf    # Daily analysis report (company, valuation, price action)
│
└── README.md
```

---

## 📊 `Star Cements.xlsx` — Model Structure

The workbook is organised into 12 linked sheets, indexed on the first tab (`Index`):

| # | Sheet | Description | Purpose |
|---|-------|-------------|---------|
| 1 | **Assumptions** | Company overview, key operating/DCF assumptions, valuation output summary | Starting point / control panel |
| 2 | **Historical** | 5-year audited financials, FY2022–FY2026 | Base data |
| 3 | **Model** | Integrated 3-statement forecast, FY2027–FY2036 | Core model |
| 4 | **Ratio Analysis** | Historical + forecast ratio dashboard (profitability, liquidity, leverage, efficiency) | Performance metrics |
| 5 | **Scenario Analysis** | Base / Bull / Bear revenue-growth scenarios and resulting DCF outputs | Sensitivity |
| 6 | **Comps** | Peer trading comparables (EV/Sales, EV/EBITDA, P/E) | Relative valuation |
| 7 | **Comp Data** | Raw financial data for the 12-peer cement universe | Source for Comps |
| 8 | **WACC** | Cost of equity (CAPM) and cost of debt build | Discount rate |
| 9 | **Beta** | Regression-based beta derivation vs. peer set | Beta input to WACC |
| 10 | **Market Data** | CMP, market capitalisation, peer share prices | Market reference |
| 11 | **Football Field Analysis** | Valuation range across all methodologies | Summary visual |

### Key Model Assumptions
- **Forecast horizon:** FY2027–FY2036 (10-year explicit period)
- **Revenue growth (Base Case):** 13.00% in FY2027, tapering 10% p.a. to ~5% by FY2036
- **COGS:** 15.56% of revenue (3-yr historical average)
- **Depreciation:** 15.22% of opening PP&E, stepped up 2.00% every 3 years from FY2030
- **Capex:** Scaled to the capacity-expansion plan (9.7 → 16.7 MTPA by FY29) — peaks at 28.23% of revenue in FY2028, tapering to ~2.93% by FY2036
- **Working capital:** DSO 18.17 days · DIO 257.09 days · DPO 165.81 days (net CCC ≈ +109 days, reflecting cement-industry raw-material stockpiling)
- **Debt:** Frozen at ₹493.19 Cr (FY2026 level) through the forecast; no new borrowings assumed
- **Tax rate:** Starts at 25.56%, stepped up 0.50% every two years to 28.06% by FY2036

### WACC Build
| Component | Value |
|---|---|
| Risk-Free Rate (10-yr G-Sec) | 7.03% |
| Equity Risk Premium | 4.53% |
| Levered Beta (peer-average unlevered, re-levered) | 1.02x |
| Cost of Equity (CAPM) | 11.66% |
| Pre-Tax Cost of Debt | 5.79% |
| After-Tax Cost of Debt | 4.31% |
| **WACC** | **10.73%** |

### Terminal Value & Output
| Metric | Value |
|---|---|
| Terminal Growth Rate (Gordon Growth) | 4.00% |
| EV/EBITDA Exit Multiple | 15.43x (avg. of 8 large-cap peers) |
| Terminal Value — GGM (FY2036, undiscounted) | ₹21,644.38 Cr |
| Terminal Value — EV/EBITDA (FY2036, undiscounted) | ₹30,455.03 Cr |
| Blended Terminal Value | ₹26,049.71 Cr |
| Enterprise Value (DCF) | ₹11,332.52 Cr |
| Equity Value (DCF) | ₹11,115.39 Cr |
| **Intrinsic Value per Share** | **₹275.99** |
| Current Market Price (as of 10 Aug 2026) | ₹198.94 |
| Implied Upside | **+38.7%** |
| Recommendation | **BUY** |

### Peer Set (Comps)
UltraTech Cement, Grasim Industries, Ambuja Cements, Shree Cement, J K Cements, Dalmia Bharat, ACC, The Ramco Cement, JSW Cement, Nuvoco Vistas, India Cements, JK Lakshmi Cement.

---

## 📄 `Star_Cement_Daily_Analysis_Report.pdf`

A daily-format research note summarising:
- Company overview and North-East India expansion strategy
- 5-year historical financials and key ratios (P/E, EV/EBITDA, RoE, RoCE)
- Shareholding pattern (promoter/public/institutional split)
- Peer valuation comparison
- Full DCF walkthrough and scenario analysis
- Price action snapshot (LTP, day/52-week range, volume, analyst target)

---

## 📈 `Star_Cement_Weekly_Returns.xlsx`

Tracks weekly stock price returns for STARCEMENT, used to monitor actual price performance against the DCF-implied intrinsic value and analyst targets over time.

---

## 🗂 `Annual Reports/`

Source filings (annual reports, investor presentations) used as the primary data inputs for the Historical sheet and Assumptions build.

---

## Methodology Notes

- All historical figures (FY2022–FY2026) are sourced from Star Cement's audited financial statements.
- Peer/market data is sourced from NSE/BSE filings and Yahoo Finance, current as of the model preparation date.
- The model uses a blended terminal value (simple average of Gordon Growth and EV/EBITDA exit-multiple methods), discounted via XNPV at WACC.
- Only the top-line revenue growth assumption differs across the Base/Bull/Bear scenarios; all other operating assumptions are held constant.

---

**Prepared by:** Anuj Patel
**Last updated:** 11 August 2026
