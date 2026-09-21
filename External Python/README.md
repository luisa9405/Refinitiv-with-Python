# External Python · Workspace data access

These are the repository's **original notebooks for locally executed Python**. They are retained in their existing format, not silently migrated to the newer Data Library.

## Connection models

- **Workspace Desktop connection:** Launch an authorised Workspace desktop application on the **same computer** running your local Python session. Install the library required by the selected notebook, then establish the session using your own credentials/app-key configuration as documented for that library.
- **Direct LSEG Data Platform connection:** A different authentication and entitlement model; it is **not** automatically enabled by having Workspace access and is **not** the required route for these examples.

Some existing notebooks use the **legacy `eikon`** Python library; others also reference `refinitiv.data`. Read the first cells of each notebook for its requirements. They have not all been migrated or execution-tested against your current installation.

## Available notebooks

- [1. Access Key Generator for Refinitiv.ipynb](1.%20Access%20Key%20Generator%20for%20Refinitiv.ipynb) — Access-key / authentication walkthrough.
- [2.Variable Code Finder in Refinitiv.ipynb](2.Variable%20Code%20Finder%20in%20Refinitiv.ipynb) — Data-item code discovery.
- [3.Historical Financial Data Downloader.ipynb](3.Historical%20Financial%20Data%20Downloader.ipynb) — Historical financial-statement extraction.
- [4.PythonStock. Historical Stock Prices Downloads.ipynb](4.PythonStock.%20Historical%20Stock%20Prices%20Downloads.ipynb) — Historical stock-price extraction.
- [5.Identify all companies in a country in Refinitiv via python.ipynb](5.Identify%20all%20companies%20in%20a%20country%20in%20Refinitiv%20via%20python.ipynb) — Companies by headquarters country.
- [6.Peer Analysis .ipynb](6.Peer%20Analysis%20.ipynb) — Peer comparison.

## Getting started

1. Install Python and JupyterLab (or use VS Code with its Jupyter extension).
2. Install the Python packages actually imported in the selected notebook, such as `pandas`, `eikon` or `refinitiv-data` as appropriate.
3. Start and sign in to Workspace Desktop when using a Desktop Session; enter **your own** authorised app-key configuration if required by that notebook/library.
4. Copy the example notebook to your research project, check data items in CodeCreator, and adjust company identifiers, parameters and local output paths.

**Security:** Never commit real keys, `.env` files, downloaded licensed datasets or output containing non-public information. Prefer environment variables or your institution's approved credential mechanism. The original notebooks in this folder have not been edited by the companion CodeBook update package; review any saved notebook outputs and example credential values separately.
