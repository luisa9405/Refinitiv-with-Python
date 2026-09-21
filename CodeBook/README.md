# CodeBook · Integrated Python in LSEG Workspace

These self-contained notebooks are intended to be run **inside CodeBook**, the notebook environment integrated with Workspace. You do not need a separate local Python installation to follow them. The examples use the `refinitiv.data` library and the permissions available to your Workspace account.

## Before starting

Open Workspace → CodeBook; create/open a notebook in the project, copy/upload the notebook you want, and execute its cells from top to bottom. The notebook opens a session via `rd.open_session()`. If your CodeBook environment has already opened a session, adapt that cell to your environment.

The `output/` directory is created within the notebook's current working directory. You may need to **download resulting CSVs** from CodeBook to your computer. The `.gitignore` at the repository root excludes generated outputs from version control.

## Tutorials

| Notebook | What you learn | Output |
|---|---|---|
| [01 · Companies by country](01_Companies_by_Country.ipynb) | `SCREEN()`, headquarters-country filters, alphabetical ordering and organization identifiers | `companies_spain.csv` |
| [02 · Company information](02_Company_Information.ipynb) | Retrieve a company profile and repeat the same request for multiple RICs | `company_profiles_spain.csv` |
| [03 · Financial data and monthly prices](03_Financial_Data_and_Monthly_Prices.ipynb) | Annual financial fields vs. monthly stock-price observations and date/frequency parameters | `financial_data_spain.csv`, `monthly_prices_spain_2024_2025.csv` |

## Concepts that matter for research

- A headquarters-country filter selects firms with headquarters in that country; it does **not** establish all countries in which a multinational operates.
- A **RIC** identifies an instrument; an **organization PermID** identifies an organization. One organization can be associated with multiple instruments.
- `FY0` refers to a fiscal reporting period; `Frq="M"` with a market-price field requests **monthly market observations**, not monthly accounting statements.
- Validate field names, field availability, business classification, reporting dates and units in **CodeCreator / Data Item Browser**. The returned column labels may differ between fields or environments.
- Compare extracts with Workspace Screener using matching selection criteria. Results, licensing and coverage can change over time.

**No access credentials, exported licensed data, or proprietary screenshots are included.** These notebooks have been validated for notebook structure and Python syntax but have **not been executed against a live LSEG session**. Confirm data-item codes and entitlement coverage in your own Workspace environment.
