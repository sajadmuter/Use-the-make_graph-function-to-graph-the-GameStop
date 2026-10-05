# Apple Stock Data Exploration

A Python learning exercise that retrieves Apple stock history and plots its opening price.

## Learning question

How can a stock price dataset be retrieved, inspected, and plotted with Python?

## Current file

[`FINL.ipynb`](FINL.ipynb)

## What the notebook does

1. Creates a yfinance ticker for Apple.
2. Downloads an Apple company-information JSON sample.
3. Reads the company information and retrieves its country field.
4. Retrieves historical stock prices.
5. Resets the index.
6. Plots the Open price against Date.

## Tools

Python, Jupyter, yfinance, pandas, matplotlib, and matplotlib-inline.

## Sources

- Stock prices: Yahoo Finance through yfinance.
- Company information: an `apple.json` sample hosted by IBM Skills Network.
- See `DATA-SOURCES.md` and `THIRD_PARTY_NOTICES.md`.

## Local setup

Install the dependencies listed in `requirements.txt`:

```bash
python -m venv .venv
# Windows (PowerShell or Command Prompt):
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe -m jupyter lab
# macOS / Linux: use .venv/bin/python instead.
```

Use the Python executable inside `.venv` for installation and launch. Open `FINL.ipynb`.

The notebook downloads the JSON sample through Python with a 30-second timeout. No wget installation is required. The historical price cutoff is 2024-10-05, with auto_adjust=False explicitly selected.

Dependencies are listed, not version-locked. Live-source execution has not been verified.

## Results and limitations

Old output cells were cleared. Helper checks passed using synthetic fixtures, and all code cells were exercised in order using mocked downloads and stock history. Live-source execution has not been verified.

This is descriptive exploration. It does not establish a relationship between business performance and share prices, produce a forecast, or demonstrate employer business impact.

## Improvements before portfolio use

- Document retrieval dates and external data usage terms.
- Restart and run all cells against the live sources.
- Add a verified chart preview and three evidence-based observations.

## Attribution and rights

The external sample data retains its source terms. No ownership of third-party data or course material is claimed.

## Offline checks

Run `python validate_analysis.py` in the installed environment. These checks use synthetic data and do not validate remote availability or market accuracy.
