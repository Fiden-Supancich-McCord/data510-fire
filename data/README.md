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

## Dataset registry

### Dataset 1: LandMark

- **Source:** [URL](https://landmarkmap.org/data-methods/access-data)
- **License:** Creative Commons -- Attribution-ShareAlike 4.0 International. Responsible non-commercial use
- **Date pulled:** 2026-05-29
- **Approximate size:** 20104 USA rows, ~2GB total (all countries)
- **Owner on this project:** LandMark's Steering Group (consortium of local, regional, and international groups)
- **Where it lives in this repo:** Raw file too large - lives on local system.
- **Ethics / consent notes:** No PII, ensure that results will not negatively impact Indigenous Peoples or local communities.
- **How to fetch (for a teammate cloning fresh):** One-time download from source.

### Dataset 2: Global Biodiversity Information Facility (GBIF)

- **Source:** [URL](https://doi.org/10.15468/dl.a9m8pz)
- **License:** CC BY-NC (non-commercial with attribution) at most strict
- **Date pulled:** <YYYY-MM-DD>
- **Approximate size:** 23571 OR rows, 14645 KB
- **Owner on this project:** GBIF Secretariat
- **Where it lives in this repo:** Raw file lives on local system, cleaned version (unnecessary columns or columns including PII removed) at `data/new_gbif_dataset.csv`
- **Ethics / consent notes:** PII from individual entries has been removed before uploading. Occurrence records here do not represent a complete census of the species we're looking at, and our chosen species do not represent the whole of Oregon's biodiversity - need to be mindful of using these results as an indicator and not unbiased truth. More occurences were recorded in locations that are more accessible and/or more densely populated. 
- **How to fetch (for a teammate cloning fresh):** One-time download from source, can use our generated DOI to get our species, time, and location specifications.

### Dataset 3: NIFC InFORM Fire Occurence Data Records

- **Source:** [URL](https://data-nifc.opendata.arcgis.com/datasets/nifc::inform-fire-occurrence-data-records/about)
- **License:** Free for strategic use. 
- **Date pulled:** 2026-06-15
- **Approximate size:** 1221418 rows, ~580MB
- **Owner on this project:** National Interagency Fire Center (NIFC)
- **Where it lives in this repo:** Raw file lives on local system. Cleaned version also lives on local system as it is still too large. 
- **Ethics / consent notes:** No PII. May not necessarily represent a complete record, as some fires in the IFPH dataset do not have a matching unique identifier in the InFORM dataset. 
- **How to fetch (for a teammate cloning fresh):** One-time download from source.

### Dataset 4: NIFC Interagency Wildland Fire Perimeter History (IFPH)

- **Source:** [URL](https://data-nifc.opendata.arcgis.com/datasets/nifc::interagencyfireperimeterhistory-all-years-view/about)
- **License:** Free for strategic use. 
- **Date pulled:** 2026-05-29
- **Approximate size:** 4262 OR rows, ~760MB total (USA)
- **Owner on this project:** National Interagency Fire Center (NIFC)
- **Where it lives in this repo:** Raw file lives on local system. Cleaned version at `data/ifph_clean`.
- **Ethics / consent notes:** No PII. Does not represent a complete record, as many fires did not have their perimeters fully mapped (including many of those that are represented in the InFORM dataset). 
- **How to fetch (for a teammate cloning fresh):** One-time download from source.

### Dataset 5: Historic Vegetation

- **Source:** [URL](https://geohub.oregon.gov/datasets/oregon-geo::historic-vegetation/about)
- **License:** CC0 1.0 License (Public domain, no copyright)
- **Date pulled:** 2026-05-29
- **Approximate size:** 43729 rows, ~161MB
- **Owner on this project:** State of Oregon
- **Where it lives in this repo:** Raw file lives on local system. 
- **Ethics / consent notes:** No PII. As a historic record, may not represent completely up-to-date ecology of Oregon. Primarily combined with GBIF occurence data to provide a more complete picture and for context about Oregon's ecology in general (e.g. what areas are forest vs. marsh vs. desert).
- **How to fetch (for a teammate cloning fresh):** One-time download from source.
