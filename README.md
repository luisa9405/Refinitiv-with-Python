# Refinitiv / LSEG with Python


## How to Cite This Repository

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22881554.svg)](https://doi.org/10.5281/zenodo.22881554)

If you use these Python notebooks, code examples, or teaching materials
in your research, academic publications, or educational activities,
please cite this repository.

**Recommended citation (APA style):**

Rodríguez-Fajardo, L. M. (2026). *Refinitiv with Python: Educational
Research Tutorials* (Version 1.0.0). Zenodo.
https://doi.org/10.5281/zenodo.22881554

**BibTeX:**

```bibtex
@software{rodriguezfajardo2026refinitiv,
  author    = {Rodríguez-Fajardo, Luisa María},
  title     = {Refinitiv with Python: Educational Research Tutorials},
  year      = {2026},
  version   = {1.0.0},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.22881554},
  url       = {https://doi.org/10.5281/zenodo.22881554}
}
```

**Data attribution:** LSEG is the provider of the financial data accessed
through these tutorials. Please acknowledge and cite LSEG separately
as the data source, in accordance with your institution's data-use
requirements.

**Financial data for research · From data discovery to reproducible access with Python**

Educational Jupyter notebooks for researchers using **LSEG Workspace (formerly Refinitiv Workspace / Eikon)**. Learn to find the correct company or instrument, select documented data items, and retrieve corporate, financial, and market information with Python.

> **Seminar slides:** [Financial data for research — Introduction to Workspace (PDF)](PDF_Introduction.pdf). The repository owner maintains the general-audience version of the presentation at this path.

## Choose your working environment

| | [External Python](External%20Python/) | [CodeBook](CodeBook/) |
|---|---|---|
| Where Python runs | On your computer (e.g., Jupyter or VS Code) | In the cloud-hosted notebook environment integrated into Workspace |
| Setup | Install and manage a local Python environment | Use the Python libraries available in CodeBook |
| Connection | Usually a **Desktop Session** through an authorised, running Workspace application for the examples in this repository | A Workspace-connected session in the CodeBook environment |
| Where output files are saved | On your local machine | In your CodeBook project; download files when needed |
| API use | Yes | **Yes — CodeBook also uses data APIs** |

**Important distinction:** Running Python outside CodeBook does **not**, by itself, mean having a separate, direct LSEG Data Platform subscription. A local Python notebook can connect through Workspace Desktop. A direct platform session is another access route and requires the corresponding credentials and entitlements.

## Follow the research workflow

1. **Discover:** Search companies, instruments, markets, and identifiers in Workspace. Distinguish a company/entity from its listed securities.
2. **Define:** Locate the exact data-item codes and parameters using Data Item Browser (DIB) and CodeCreator.
3. **Retrieve:** Run the appropriate notebook in [CodeBook](CodeBook/) or [External Python](External%20Python/).
4. **Document:** Record the identifiers, screening criteria, fields, dates, reporting frequency, currency, scaling and extraction date used in your study.

## Tutorials

### [01 · External Python](External%20Python/)

Original local-Python notebooks on authentication, data-item discovery, historical financial statements, historical stock prices, company screening, and peer analysis. Some notebooks use the **legacy `eikon` library**; check their specific requirements and authentication method before executing them.

### [02 · CodeBook](CodeBook/)

Hands-on examples using `refinitiv.data` in the integrated Workspace environment:

- [01 — Companies by country](CodeBook/01_Companies_by_Country.ipynb)
- [02 — Company information](CodeBook/02_Company_Information.ipynb)
- [03 — Financial data and monthly prices](CodeBook/03_Financial_Data_and_Monthly_Prices.ipynb)

The tutorials are educational examples, **not pre-extracted datasets**. Their results depend on the current data, the requested instrument, access permissions and the specific field definitions.

## Research and responsible use

Access and coverage depend on institutional permissions and LSEG data entitlements. Verify company/entity versus instrument identifiers, fiscal period-end dates, units, currencies, field definitions, and the date of extraction before using observations in empirical research. **Do not upload licensed downloaded data, institution-specific files, passwords, API keys, app keys, or tokens to this public repository.**

This is an independent educational repository and is not an official LSEG product or an endorsement by LSEG.

## Author

**Luisa María Rodríguez-Fajardo**  
PhD Candidate in Business Administration · University of Chile

Feedback and educational contributions are welcome through GitHub Issues and Pull Requests.
