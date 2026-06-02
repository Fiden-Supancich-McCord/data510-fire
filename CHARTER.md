# Studio Charter: Fire!

> Filled in live during the **Studio Charter** session in week 3. Every section below is committed in the same commit at the end of that class block. See [Studio Charter (single-session inception)](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for the script and time-boxes.

**Owner team:** Amaya Supancich-McCord, Spencer Fiden

**Owner Product Lead:** Co-lead

**Peer Stakeholder POs:** Brooke Proctor, Serena Walter, Siera Edwards

**Instructor / Sponsor:** Lucas Cordova (`LucasCordova` on GitHub)

**GitHub repo:** [link](https://github.com/Fiden-Supancich-McCord/data510-fire)

**GitHub Projects board:** [link](https://github.com/orgs/Fiden-Supancich-McCord/projects/1/views/1)

**Discord category:** `#Project-5: Amaya & Spencer`
**Studio Session:** 1
**Studio formed:** 06/01/2026

## Vision

Existing wildfire and forest resilience studies often examine vegetation structure or fire severity independently, while fewer accessible data science projects integrate Indigenous stewardship geography, biodiversity indicators, and wildfire outcomes into a reproducible geospatial analysis framework for the West Coast and PNW. Our vision a world with more integrated biodiversity, stewardship, and fire prevention methods.

## Mission

If successful, our project can help prioritize ecological restoration strategies and identify landscape characteristics associated with reduced fire severity.

## Context

- **Users / affected parties:** local communities, wildfire-prone regions, Indigenous leadership/fire strategists, state/federal land management agencies, and researchers in forestry, ecology, and wildfire resilience planners. 
- **Data sources (proposed):** USGS, USDA, Wildfire Risk to Communities (USDA associated), direct contact with tribes (send email).
- **Constraints:** no GIS experience (lots of data is just GIS data). 
- **Ethics risks:** Using CARE & FAIR principles for Indigenous data governance as relevant frameworks. Acknowledge depth & often qualitative nature of Indigenous ecological knowledge and that tribal knowledge may be restricted, contextual, or not intended for outside use/extraction. 

## Success criteria by milestone

- **M1, proposal (W4):** Knowing all/most data sources & a solid plan for ingestion (ideally tabular format). 
- **M2, data summary (W7):** Descriptive statistics for all of our data sources & a solid plan for how to clean & bridge them.
- **M3, poster rough draft (W10):** Most analytical findings agreed upon, a layout and plan for finalized graphics, and a shared understanding of limitations, interpretability, and future research/expansion. 
- **M4, write-up rough draft (W12):** Have a well-considered answer for our research question & analysis to support our interpretation. 
- **M5, final write-up and poster (W14):** Win! Succeed! People are able to take our interpretations and move forward with them in their own departments, learning new information that would otherwise be difficult to find or compile.

## Working agreements (internal to owner team)

- **Sync rhythm:** Have swim lanes decided (tentatively) by Saturday at noon. Check in on Thursday (async) and Saturday (tentatively in person), provide other async updates as needed. Project specific messages are DMs. 
- **Code review:** Review before Saturday check-in. Otherwise, ensure we have good documentation and are on the same page before Monday class. 
- **Decision rule:** Have a conversation, ensure both people are listening to each other's points of view (no immediate shut downs, consider constraints and possibilities). If a decision really can't be reached, talk to outside perspectives (peer POs and/or Prof Cordova). 

## Working agreements (triad with peer POs)

- **Studio Brief due:** 5pm Sunday before class, committed to `studio/briefs/W<NN>-<peer>.md` and linked in `#<project>-studio` on Discord. 
- **Studio Critique due:** Midnight Wednesday or earlier if possible, committed to `studio/critiques/W<NN>-<peer>.md` and linked in `#<project>-studio` on Discord.
- **Priority conflict resolution:** owner team integrates briefs in good faith; the instructor arbitrates (as Process Expert) if peer POs and owner team disagree.

## Response SLAs (Service Level Agreements)

A **Service Level Agreement** is a written promise the triad makes about *how fast* each side responds when a specific signal arrives. Every row must have an answer before this Charter is committed. See [Response SLAs](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html#response-slas-service-level-agreements) for the full definition.

| When this signal arrives... | Who responds | By when |
|-----------------------------|--------------|---------|
| Peer PO files a **Studio Brief** (commits to `studio/briefs/...`, links in `#project-5-studio`) | Owner team | By Monday before 6pm |
| Peer PO files a **Studio Critique** | Owner team | By Saturday at noon |
| Owner team posts an **Iteration Review** in `README.md` | Both peer POs | read before filing the next Brief and Critique |
| Owner team flags a **blocker** in `#project-5-blockers` | Instructor, plus any tagged peer PO | (owner team sends a gchat if you want quick response) responds by the next Studio Session at the latest; faster if online |
| Anyone asks a clarifying question in `#project-5-general` | Whoever is tagged (default: owner team) | ownder team must send a text for quick response, reply within 48 hours, even if the reply is "we will look at this next iteration" |

## Definition of Ready (PBI)

A PBI is ready to be pulled out of `Backlog` and moved into `Create` when it has:

- A one-sentence hypothesis or user story.
- A named **Create**, **Observe**, **Analyze** triple.
- A milestone tag (`M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`).
- A plant size estimate (Seed, Flower, Tree, Forest).
- WIP slack on the board: `Create + Observe + Analyze` is below the team's WIP cap (owners + 1).

## Definition of Done (PBI)

A PBI is done, and may be moved from `Analyze` into `Done`, when:

- The Create artifact is in the repo or linked from the issue.
- The Observe results are recorded somewhere referenceable (notebook output, processed dataset, draft results section).
- The Analyze writeup names a next step (continue, pivot, kill, or decompose into new PBIs).
- A peer PO has either signed off in `#project-5studio` or filed a Studio Critique covering it.
- The card is linked under *Completed PBIs* in the next Iteration Review in `README.md`.

## Context map

> Optional. Replace this block with a Mermaid `flowchart LR` showing how users, data, constraints, and ethics risks flow into the owner team and out to the capstone outcome. See the [`charter-inception.qmd` template](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for a starting Mermaid diagram.

## Stakeholder alignment memo (one-page summary)

### Why we exist
Few accessible data science projects integrate Indigenous stewardship geography, biodiversity indicators, and wildfire outcomes into a reproducible geospatial analysis framework for the West Coast or PNW. If successful, our project can help prioritize ecological restoration strategies and identify landscape characteristics associated with reduced fire severity.

### What we will deliver to peer POs every week
- An Iteration Review in this `README.md` by Saturday at 5pm.
- A summary of which Studio Brief items we adopted, deferred, or declined and why

### What we need from peer POs every week
- A Studio Brief by Sunday at 5pm next class (next iteration's requirements, questions, risks)
- A Studio Critique by Wednesday at midnight next class (assessment of last week's delivery)

### How to reach us
- Discord category: `#<project>-general` (day-to-day), `#<project>-studio` (Briefs and Critiques), `#<project>-blockers` (impediments)
- GitHub repo: [link](https://github.com/Fiden-Supancich-McCord/data510-fire)
- GitHub Projects board: [link](https://github.com/orgs/Fiden-Supancich-McCord/projects/1/views/1)
