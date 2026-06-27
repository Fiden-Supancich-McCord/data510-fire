# <Analyzing Biodiversity and Wildfire Outcomes on Indigenous and Non-Indigenous Lands Across Oregon>

## Quick reference

| Field | Value |
|-------|-------|
| Owner team | Amaya Supancich-McCord & Spencer Fiden |
| Owner Product Lead | Spencer Fiden |
| Peer Stakeholder POs | Brooke Proctor, Serenna Walter, & Siera Edwards |
| Studio Session | 1 |
| GitHub repo | https://github.com/Fiden-Supancich-McCord/data510-fire |
| GitHub Projects board | https://github.com/orgs/Fiden-Supancich-McCord/projects/1 |
| Discord category | `#5` |
| Instructor / Sponsor | Lucas Cordova (`LucasCordova` on GitHub) |

## What this repo contains

| Path | Purpose |
|------|---------|
| [`CHARTER.md`](CHARTER.md) | Studio Charter: vision, mission, context, success criteria, working agreements, SLAs, DoR / DoD. Committed at the end of the week 3 Studio Charter session. |
| [`BACKLOG.md`](BACKLOG.md) | Human-readable mirror of the GitHub Projects board. |
| [`studio/briefs/`](studio/briefs/) | Weekly Studio Briefs from peer POs (`W<NN>-<peer>.md`). |
| [`studio/critiques/`](studio/critiques/) | Weekly Studio Critiques from peer POs (`W<NN>-<peer>.md`). |
| [`src/`](src/) | Working code (scripts, modules). |
| [`notebooks/`](notebooks/) | Exploratory and reporting notebooks. |
| [`data/`](data/) | Project data. Raw inputs are `.gitignored` by default; see `data/README.md`. |
| [`deliverables/`](deliverables/) | Milestone deliverables: proposal, data summary, poster, write-up. |

## How this project runs (DS3 in one paragraph)

This project is run as a **DS3 studio**: the owner team is paired with two or three **peer Stakeholder POs** drawn from adjacent capstone projects. Every week the peer POs file a **Studio Brief** for the next iteration and a **Studio Critique** of the last iteration. The owner team commits an **Iteration Review** here in `README.md` before each class. See the [Studio Session weekly ritual](https://courses.lpcordova.phd/data510/project-framework/weekly-ritual.html) for the cadence and [Studio Charter](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for the inception session.

---

# Iteration Reviews

One subsection per class week. The owner team commits the new section **before each class** so peer POs can read it before filing the next Brief and Critique. Use the template at the bottom of this file for any extra weeks you add.

## Week 4 -- Proposal milestone (M1)

**Iteration ending:** 5/31

**Milestone tag in focus:** `M1-proposal`

**Completed PBIs**
- Contact Jason Henry (note: decided against GIS route, no longer applicable)

**In-flight (carrying across the boundary)**
- Decide on top three datasets (Analyze)
- Research working with shape files (Create)
- Acquire and document our prioritized datasets (Create)
- Data sources and access plan (Create)

**Stakeholder response log**
- Studio Brief from Serenna: adopted = Shapefiles, deferred = Ethics on Indigenous Data & Underbrush and Debris Data
- Studio Brief from Brooke: adopted = Prioritized Datasets & Data Cleaning Breakdown, deferred = Prioritized Ethics
- Studio Brief from Siera: adopted = Keep Focusing on data that will answer your research question & Decide on your project scope & Break into the shape file data (if any) early

**Plan for next iteration**
- Top PBIs (with milestone tags):
    - Acquire/document LandMark, GBIF data
    - handle data sources and access plan
    - plan our analysis
  
**Risks and impediments**
- busy (wedding, one member out of town Thurs-Sun next week)

## Week 5

**Iteration ending:** 6/7
**Milestone tag in focus:** `M1-proposal` / `M2-data-summary`

**Completed PBIs**
- Write up project proposal
    - Data sources and access plan
    - Ethics and risk notes
    - Create data engineering plan
    - Draft research question and frame as a testable claim

**Stakeholder response log**
- NA

**Plan for next iteration**
- Acquire/document data
- Research working with shapefiles/develop workflow for shapefiles

**Risks and impediments**
- Shapefiles scary, workflow may be complex (espeically if we move between R and Python)

## Week 6

**Iteration ending:** 6/14
**Milestone tag in focus:** `M2-data-summary`

**Completed PBIs**
- Decide on our top three datasets (we have 4)
- Research working with shapefiles

**In Progress**
- Acquire/document datasets
    - Interagency Fire Perimiter History is done
    - LandMark is done
- Research which land cover species are most applicable
- Data cleaning

**Stakeholder response log**
- NA

**Plan for next iteration**
- Continue acquiring/documenting datasets
- Make progress on data cleaning!
- Begin at least masterminding the grid cells

**Risks and impediments**
- Data quality issues (missingness, few entries for certain species in GBIF, etc.)
- Engineering grid cells (and their respective tables) may be challenging

## Week 7 -- Data summary milestone (M2)

**Iteration ending:** 6/27

**Milestone tag in focus:** `M2-data-summary`

**Completed PBIs** 
- Siera: Create Shapefile for Streams
- Serenna: Clean EAB Data
- Serenna: Get new EAB data for Cordova and clean _(hypothetically by Sunday evening)_
- Brooke: Scrape Tree Data _(hypothetically by Sunday evening)_
- Add data we have to the repository _(hypothetically by Sunday evening)_
- Data cleaning _(hypothetically by Sunday evening)_
- Exploratory Data Analysis _(hypothetically by Sunday evening)_

**Stakeholder response log**
- NA

**Plan for next iteration**
- Figure out how to create an area shapefile that will connect salem_addresses and stream_shapes with the other tables. 
- Feature engineering
- Begin creating our 3 planned models

**Risks and impediments**
- We still need to figure out how to connect salem_addresses and stream_shapes with our other data. Through the process of doing our data summary, we found that it was impossible to get Salem zipcodes due to a paywall. We will need to somehow create our own shapefile that shows the density of addresses. This will be used to connect salem_addresses and stream_shapes to our other datasets.
- Origianlly in our project proposal, we were hoping to have feature engineering completed by this iteration. However, as previously mentioned, we were unable to complete feature engineering by the Data Summary deadline due to the extensive process that webscraping our data ended up becoming. We are now lumping feature engineering into the modeling process. This is a risk due to it simply being more to do before the poster draft. 

**Retrospective (milestone boundary)**
- What worked: The stream, temperature, and weather data were all colleted successfully. The Tree Plotter and EAB data were a lot more challenging and we needed help from Professor Cordova to collect. 
- What did not: EAB Sighting data is no longer useful due to only one confirmed sighting. This made us need to pivot how we were collecting the main data source for EAB. 
- One change for next iteration: Implement plan for data density connection to other datasets.

## Week 8

**Iteration ending:** <date>
**Milestone tag in focus:** `M3-poster-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 9

**Iteration ending:** <date>
**Milestone tag in focus:** `M3-poster-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 10 -- Poster rough-draft milestone (M3)

**Iteration ending:** <date>
**Milestone tag in focus:** `M3-poster-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

**Retrospective (milestone boundary)**
- What worked: ...
- What did not: ...
- One change for next iteration: ...

## Week 11

**Iteration ending:** <date>
**Milestone tag in focus:** `M4-writeup-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 12 -- Write-up rough-draft milestone (M4)

**Iteration ending:** <date>
**Milestone tag in focus:** `M4-writeup-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

**Retrospective (milestone boundary)**
- What worked: ...
- What did not: ...
- One change for next iteration: ...

## Week 13

**Iteration ending:** <date>
**Milestone tag in focus:** `M5-final`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 14 -- Final write-up and poster (M5)

**Iteration ending:** <date>
**Milestone tag in focus:** `M5-final`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Final retrospective**
- What worked: ...
- What did not: ...
- What we would change if we ran this project again: ...

---

## Iteration Review template (copy for any extra week)

```markdown
## Week <NN>

**Iteration ending:** <date>
**Milestone tag in focus:** <M1-proposal | M2-data-summary | M3-poster-draft | M4-writeup-draft | M5-final | infra | ethics>

**Completed PBIs**
- ...

**In-flight (carrying across the boundary)**
- ...

**Stakeholder response log**
- Studio Brief from <peer PO>: adopted = ..., deferred = ..., declined (with reason) = ...

**Plan for next iteration**
- Top PBIs (with milestone tags): ...

**Risks and impediments**
- ...
```
