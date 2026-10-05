# Data Sources

- Apple stock history: Yahoo Finance, accessed with `yf.Ticker("AAPL").history(period="max")`.
- Company information sample: https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/data/apple.json

The notebook reads the sample's country field and plots historical Open prices.

Document the retrieval date, coverage, adjustment settings, transformations, and source usage terms before presenting a reproducible analysis. The commit date is not evidence of the download date.

The notebook downloads `apple.json` at runtime. No separate JSON sample is currently tracked in the repository root.

No confidential telecom or warehouse data is used by the inspected notebook.

## Refactored retrieval settings

Price retrieval sets auto_adjust=False explicitly. The notebook declares a fixed cutoff. No new live download date is claimed; source availability and coverage must be recorded after a successful live run.
