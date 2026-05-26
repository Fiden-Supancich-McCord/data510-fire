# Backlog: <project name>

This file is the **human-readable mirror** of the [GitHub Projects (v2) Iterative Development board](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) for this repo. Every row here is also a GitHub issue, added to the board, tagged with a milestone label, and sized.

## Conventions

- Each item has: id, title, hypothesis or user story, **Create / Observe / Analyze** triple, milestone tag, size.
- Items are ordered top to bottom by **priority**.
- Milestone tags: `M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`.
- Sizes: Seed, Flower, Tree, Forest.
- The board has five columns: `Backlog` → `Create` → `Observe` → `Analyze` → `Done`. Each column is the *phase of work happening on a single PBI right now*, not a work type. See the [Iterative Development board explainer](https://courses.lpcordova.phd/data510/project-framework/#github-projects-board-per-project-iterative-development-board) for what each column means and when to advance a card.
- WIP cap: `Create + Observe + Analyze` ≤ `owners + 1` at any time.
- Definition of Ready and Definition of Done live in [`CHARTER.md`](CHARTER.md).

## Items

### PBI-001

- **Title:** Decide on our top three datasets to determine if they are usable.
- **Hypothesis:** Three datasets are the most relevant to our research question and should be prioritized.
- **Create:** updated items in our backlog with specific datasets to look into
- **Observe:** there's three of them
- **Analyze:** determine if these adequately answer our research question or if we need more/backup sources
- **Tag:** `M1-proposal`
- **Size:** Seed
- **GitHub issue:** <link once filed>

### PBI-002

- **Title:** Acquire and document our prioritized dataset
- **Hypothesis:** the dataset is accessible, license-compatible, and large enough to answer our research question.
- **Create:** ingestion script and `data/README.md` section describing schema.
- **Observe:** row counts, missingness, key uniqueness, distribution sanity checks.
- **Analyze:** decide whether the dataset survives feasibility; document in the next Iteration Review.
- **Tag:** `M1-proposal`
- **Size:** Tree
- **GitHub issue:** <link once filed>

### PBI-003

- **Title:** Draft research question and frame as a testable claim
- **Hypothesis:** We can state the project's research question in one sentence that names the population, the predictor or treatment, and the outcome.
- **Create:** RQ statement in `CHARTER.md` Mission section; one-paragraph framing in the proposal draft.
- **Observe:** can a peer PO who has never seen the project repeat the question back accurately?
- **Analyze:** revise based on Studio Brief feedback.
- **Tag:** `M1-proposal`
- **Size:** Flower
- **GitHub issue:** <link once filed>

### PBI-004

- **Title:** Contact Jason Henry (Brooke's contact) to ask about GIS
- **Hypothesis:** we can use GIS! 
- **Create:** updated backlog with steps for accessing GIS
- **Observe:** 
- **Analyze:** can we feasibly learn to use GIS within the timeframe of this project? Will it realistically work with what we're trying to analyze
- **Tag:** `M1-proposal`
- **Size:** Flower
- **GitHub issue:** <link once filed>

### PBI-005

- **Title:** Contact someone to ask about Grand Ronde 
- **Hypothesis:** people love to give us data
- **Create:** contact information/updated backlog
- **Observe:** 
- **Analyze:** will people actually give us data? is it in a usable format
- **Tag:** `M1-proposal`
- **Size:** Flower
- **GitHub issue:** <link once filed>

<!-- Add more PBIs below following the same shape. -->
