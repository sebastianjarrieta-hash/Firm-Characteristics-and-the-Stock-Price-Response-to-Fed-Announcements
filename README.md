Firm Characteristics and the Stock Price Response to Fed Announcements

Author: Sebastian Arrieta Perez — Texas A&M University, Date: June 2026

Overview

This paper studies why firms react differently to the same Federal Reserve announcement. On October 29, 2008, the FOMC cut rates 50bp to 1% — an identical shock hitting every public firm at once — yet stock returns in the minutes around the announcement varied widely across companies. This project asks what firm characteristics explain that cross-sectional dispersion.

Data
High-frequency intraday returns around FOMC announcements (WRDS/TAQ)
S&P 500 firm panel
Firm characteristics constructed from CRSP/Compustat:
Leverage — total debt / total assets
Tobin's Q — (book assets + market equity − book equity) / book assets
Cyclicality — rolling 20-quarter regression slope of firm YoY ROA growth on real GDP growth

Methodology

The core empirical approach follows Ottonello & Winberry (2020), decomposing each firm characteristic into:

A within-firm ("state") effect — is this firm temporarily more leveraged, higher-Q, or more cyclical than its own historical norm?
A cross-firm ("type") effect — fixed differences between firms

Both level and within-firm-demeaned specifications are estimated to separate these two channels. All coefficient interpretations are stated in within-firm terms, per the methodology's core identifying assumption.

Robustness: Results are re-estimated against two alternative monetary policy shock measures — Bauer-Swanson (2023) and Boehm-Kroner (2024) — with a 5×5 shock correlation matrix reported to show how the shock series relate to one another.

Key Findings
Cyclicality effect holds up under the CBI shock specification
Tobin's Q effect holds up under the FRN shock specification
Leverage's explanatory role is weak once cyclicality and Q are accounted for; firm size and bid-ask spread are included as controls rather than primary channels
Repo Structure
notebooks/   Python analysis notebooks (data construction, regressions, robustness checks)
tables/      LaTeX regression tables (per-shock, combined)
paper/       Full paper PDF (compiled from Overleaf)

Tools

Python (pandas, statsmodels) for data construction and regression analysis, run in Google Colab · LaTeX (Overleaf) for tables and writeup
