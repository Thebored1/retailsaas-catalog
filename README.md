# RetailSaaS Catalog Repository

This repository is the source for online product catalog data.
The desktop app fetches:

`https://raw.githubusercontent.com/Thebored1/retailsaas-catalog/main/catalog/v1/index.json`

## Structure
- `catalog/v1/index.json` (manifest)
- `catalog/v1/categories/<category>.json` (per-category products)

## Update flow
1. Edit one or more category JSON files
2. Update `catalog/v1/index.json` only when adding/removing categories
3. Commit and push to `main`
4. Desktop users click `Inventory -> Online Catalog -> Refresh Catalog`

No link pasting is required in the app.
