# CodeBook — Educational Python Tutorials

**Author:** Luisa María Rodríguez-Fajardo  
**Environment:** LSEG Workspace → CodeBook (Python)  
**Project:** [Refinitiv with Python](https://github.com/luisa9405/Refinitiv-with-Python)

## Start here

Open each `.ipynb` in CodeBook, run its cells in order, and inspect the returned data before using them in research. Examples are independent and use a few predefined instruments; no external Python installation is required. Each notebook creates an `output/` folder only when executed. Do not publish vendor-licensed data exports in the repository.

**Existing introductory notebooks (retain your current files):**

- `01_Companies_by_Country.ipynb` — Screen Spanish-headquartered companies.
- `02_Company_Information.ipynb` — Retrieve a company profile.
- `03_Financial_Data_and_Monthly_Prices.ipynb` — Fundamentals and monthly stock-price observations.

**Additional short demonstrations:**

| Notebook | Scope |
|---|---|
| [`04_Historical_Financial_Data.ipynb`](04_Historical_Financial_Data.ipynb) | Historical financial data |
| [`05_Financial_Ratios.ipynb`](05_Financial_Ratios.ipynb) | Financial ratios |
| [`06_ESG_Data.ipynb`](06_ESG_Data.ipynb) | ESG data |
| [`07_Ownership.ipynb`](07_Ownership.ipynb) | Ownership by investor category |
| [`08_Board_of_Directors.ipynb`](08_Board_of_Directors.ipynb) | Board of directors |
| [`09_Analyst_Estimates.ipynb`](09_Analyst_Estimates.ipynb) | Analyst estimates |
| [`10_Corporate_Events_Dividends.ipynb`](10_Corporate_Events_Dividends.ipynb) | Corporate events: dividends |
| [`11_Index_Constituents.ipynb`](11_Index_Constituents.ipynb) | Index constituents |
| [`12_Peer_Comparison.ipynb`](12_Peer_Comparison.ipynb) | Peer comparison |
| [`13_Macroeconomic_FX.ipynb`](13_Macroeconomic_FX.ipynb) | Macroeconomic indicators: exchange rates |
| [`14_Firm_Year_Panel.ipynb`](14_Firm_Year_Panel.ipynb) | A simple firm-year panel |

## Scope and reproducibility

These are short introductory extraction examples, **not** complete data-collection pipelines or empirical research methods. Individual data-item availability, reporting periods, date conventions, permissions and returned column labels may differ across subscriptions. Check each field in Data Item Browser / CodeCreator; a successful request does not establish a variable’s research validity.

- Fundamental values refer to fiscal reporting periods; a fixed calendar window does not guarantee the same fiscal year for every firm.
- Index constituents represent the chain snapshot at the time of request, not historical membership.
- ESG snapshots and ownership statistics should not be treated as historical point-in-time data by default.
- The firm-year notebook demonstrates the shape of an annual extract; it is not an audited balanced panel and does not merge ESG or board data.

## Citation and data attribution

If these teaching notebooks contribute to a thesis, publication or scholarly teaching material, please cite the repository using the GitHub **“Cite this repository”** link, enabled by [`CITATION.cff`](../CITATION.cff). Cite LSEG/Refinitiv separately as the underlying data provider, following your institution’s data-access and licensing conditions. Citation is requested, not an access restriction or guarantee that every user will cite.
