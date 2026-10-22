# Methods: Land Clearing, Forestry Mulching and Stump Removal Cost Register (US, 2026)

## Collection
- **Starting list:** the outbound sources cited on landclearingguide.com's live cost pages (/land-clearing-cost/, /forestry-mulching-cost/, /stump-removal-cost/), plus contractor price pages found by web search on 2026-10-21.
- **How:** each page was fetched live on 2026-10-21 (America/Chicago); the raw HTML and a text extraction were kept locally (raw/, not redistributed). Figures were recorded by hand into `src/build.py` with a short verbatim quote. The build normalizes whitespace and dashes and **fails** unless (a) the quote appears in that page's text and (b) every number in the row appears inside the quote.
- No figures came from calls, quote requests, forms, logins or paywalled content.
- **Coverage:** 58 rows from 15 source URLs and 10 independent businesses; 16 primary-tier rows and 42 secondary-tier rows; local rows cover GA, IN, NC, OR, TN, TX, UT, VA.

## Tiers and grouping
- **Primary:** a business publishing its own price, price list, or quoted/completed project.
- **Secondary:** aggregator cost guides (Angi, HomeAdvisor, HomeGuide, etc.), publishers, manufacturers, calculator sites, news reports, and contractor pages that describe general market ranges rather than their own prices.
- Angi and HomeAdvisor share `independent_business` = "Angi Inc." Multiple pages from one company share one value and are not independent corroboration.

## Rules applied
1. No averaging, blending, midpoints or estimates. Any average is the source's own stated figure.
2. Open-ended figures ("$X+", "starting at") are recorded as stated and flagged in `notes`.
3. Scope and unit are recorded with every row; compare rows only when scope, unit and geography match.
4. Undated sources are `Not stated`; dates from page metadata are labeled as such.
5. Only individual figures and short quotes are reproduced; no page text is mirrored.

## Exclusions and gaps
- Not used: angi.com forestry-mulching pages returned HTTP 403; rucciforestry.com returned an empty page; tjlandservice.com returned no content.
- Not used: bmstumpgrinding.com (prices include Canadian HST; not US/USD). leaderexcavation.com and lead-gen guides restate other guides (derivative).
- Excavation cost (landclearingguide.com/excavation-cost/) is out of scope for this version.
- Gap: primary prices only from TX, TN, GA/NC, IN and UT; no Southeast coastal, Northeast or Pacific primary sources.

## Limitations
- Published prices, not transactions; businesses choose what to publish.
- Not representative; few markets and few businesses per market.
- Aggregator ranges are national with undisclosed or partially disclosed methods.
- Point in time; re-check `source_url` before relying on a figure.
