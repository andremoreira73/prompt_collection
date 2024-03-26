# Financial check using public data

In this prompt, the user provides a table with common financial data from public sources (e.g P&L and balance sheets - available in the internet for public companies)
and asks for a summarized health check. The results with ChatGPT4 are very good, even at zero-shot.

// PROMPT 2 START //

I have a partial financial statement that I want you to analyze. The document is structured as follows:
The first few rows contain general information such as document status and period covered.
The main body starts from row X and includes key financial metrics in the first column, with subsequent columns representing different fiscal years.
The metrics of interest include Sales, EBITDA, Net Profit/Loss, Free Cash Flow, etc., each listed under specific headings.
There may be empty rows or additional notes interspersed within the data.
Based on this structure, please focus on analyzing CHANGES in the following indicators: (1) Revenues; (2) EBITDA; (3) Net profit/loss; (4) Free Cash Flow; (5) Liquidity; (6) Equity; (7) Financial gearing; (8) Ability to repay debt. Based on your analysis, draw conclusions about the company’s health and outlook.
Ready?

// PROMPT 1 END //

At this point the model will say it is ready - time to copy-paste the table. Note that, assuming these are realively small tables,
I prefer to copy-paste rather than uploading. Uploading demands that ChatGPT uses python code to read the table, and in my experience
the results were far better by simply copy-pasting the table - if it is not too big.

// PROMPT 2 START //

<copy-paste the table>

// PROMPT 2 END //

From here on, watch the model provide a really nice financial health check!





