# `data/`

Project data lives here. The repo root `.gitignore` excludes large or sensitive subfolders by default. The structure below is the convention you should follow.

```
data/
  raw/         # original inputs, never edited in place        (gitignored)
  external/    # third-party data you did not generate         (gitignored)
  interim/     # intermediate scratch outputs                  (gitignored)
  processed/   # cleaned, analysis-ready snapshots (committable if small)
  README.md    # describe each dataset: source, license, date, size
  SCHEMA.md    # describe processed dataset schemas once they stabilize
```

## What to **always** commit

- This `README.md` describing every dataset, with: source URL or contact, license, date pulled, approximate size, who in the team owns it, and any ethics / consent notes.
- A `SCHEMA.md` documenting the columns, types, and units of your processed datasets, once they stabilize.
- Small (< 1 MB) reproducible processed snapshots under `data/processed/` if your analysis depends on a specific version.

## What to **never** commit

- Personally identifiable information (PII), protected health information (PHI), or any data subject to a data use agreement that forbids redistribution.
- Credentials, API keys, OAuth tokens, or `.env` files.
- Multi-megabyte raw downloads. Document how to fetch them in this README instead.

## Dataset registry (in progress)

### Dataset 1: LandMark

- **Source:** [URL](https://landmarkmap.org/data-methods/access-data)
- **License:** Creative Commons -- Attribution-ShareAlike 4.0 International. Responsible non-commercial use
- **Date pulled:** 2026-05-29
- **Approximate size:** 20104 USA rows, ~2GB total (all countries)
- **Owner on this project:** LandMark's Steering Group (consortium of local, regional, and international groups)
- **Where it lives in this repo:** Raw file too large - lives on local system.
- **Ethics / consent notes:** No PII, ensure that results will not negatively impact Indigenous Peoples or local communities.
- **How to fetch (for a teammate cloning fresh):** One-time download from source.

### Dataset 2: <name>

- ...
