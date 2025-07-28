# Financial Health Check Using Public Data

## Description

Analyzes financial statements from public sources to provide a comprehensive health assessment of companies, focusing on key financial indicators and trends over time.

## Use Case

- Quick financial health assessment of public companies
- Investment research and due diligence
- Competitor financial analysis
- Identifying financial trends and red flags
- Credit risk assessment

## Implementation Notes

- Works best with copy-pasted financial tables
- Performs better with direct text input than file uploads
- Zero-shot prompting yields excellent results
- Supports P&L statements and balance sheets

---

## PROMPT 1

I have a partial financial statement that I want you to analyze. The document is structured as follows:
The first few rows contain general information such as document status and period covered.
The main body starts from row X and includes key financial metrics in the first column, with subsequent columns representing different fiscal years.
The metrics of interest include Sales, EBITDA, Net Profit/Loss, Free Cash Flow, etc., each listed under specific headings.
There may be empty rows or additional notes interspersed within the data.

Based on this structure, please focus on analyzing CHANGES in the following indicators:
(1) Revenues
(2) EBITDA
(3) Net profit/loss
(4) Free Cash Flow
(5) Liquidity
(6) Equity
(7) Financial gearing
(8) Ability to repay debt

Based on your analysis, draw conclusions about the company's health and outlook.
Ready?

[Wait for confirmation]

## PROMPT 2

[Copy-paste the financial table here]
