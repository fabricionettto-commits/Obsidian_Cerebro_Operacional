# Sanitized Architecture Notes

This note documents the public-safe version of the operational data architecture.

## Public Naming Rules

- Replace real vessel names with `Vessel_A`, `Vessel_B`, or `operation_table`.
- Replace customer names with `Customer_001`.
- Replace internal services/routes with `Service_A`.
- Replace database URLs with `<DATABASE_URL>`.
- Replace local absolute paths with `<LOCAL_PROJECT_DIR>`.

## Private Data Excluded From Git

- Raw spreadsheets.
- Normalized CSVs generated from private data.
- Static dashboards generated from live data.
- Daily operational memory files.
- API keys, database URLs, and service role keys.

## Safe Data To Publish

- Pipeline source code after removing private constants.
- SQL schema using generic table names.
- Documentation of architecture and design decisions.
- Small anonymized sample payloads.
- Screenshots with all names, IDs, and routes redacted.
