# Land Clearing, Forestry Mulching and Stump Removal Cost Register (US, 2026)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23550674.svg)](https://doi.org/10.5281/zenodo.23550674)

Published by **Land Clearing Guide** (https://landclearingguide.com/). This GitHub repository is a mirror; the canonical, versioned release is on Zenodo.

- **DOI:** [10.5281/zenodo.23550674](https://doi.org/10.5281/zenodo.23550674)
- **Zenodo record:** https://zenodo.org/records/23550674
- **Data page:** https://landclearingguide.com/land-clearing-cost/
- **License:** CC BY 4.0 (see LICENSE)

## How to cite
Land Clearing Guide. *Land Clearing, Forestry Mulching and Stump Removal Cost Register (US, 2026)*. Zenodo. https://doi.org/10.5281/zenodo.23550674

---

# Land Clearing, Forestry Mulching and Stump Removal Cost Register (US, 2026)

Compiled by **Land Clearing Guide** (landclearingguide.com). Version 2026-10-21. **Draft — not yet published.**

A register of individual prices that US contractors and consumer cost guides publish on public web pages for land clearing, forestry mulching, stump grinding and stump removal. Each row is one published figure with its unit, scope, geography, publisher, source URL, source date, retrieval date and a short verbatim quote of the figure.

- **File:** `land-clearing-cost-register.csv` (58 rows)
- **Coverage:** 58 rows from 15 source URLs and 10 independent businesses; 16 primary-tier rows and 42 secondary-tier rows; local rows cover GA, IN, NC, OR, TN, TX, UT, VA.
- **Build:** `python3 src/build.py` re-verifies every quote against the raw snapshots and fails if any quote or number is missing.
- **Docs:** METHODS.md, DATA-DICTIONARY.md, FINDINGS.md, raw/SOURCES.md
- **License:** CC BY 4.0 for the compilation (see LICENSE). Underlying figures belong to their publishers and are cited, not relicensed.

Not a quote, survey or representative sample. Do not average rows across different units, scopes or geographies.

Cite as: Land Clearing Guide (2026). *Land Clearing, Forestry Mulching and Stump Removal Cost Register (US, 2026)* (Version 2026-10-21) [Data set].
