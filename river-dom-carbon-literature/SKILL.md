---
name: river-dom-carbon-literature
description: Use when the user asks to search, screen, summarize, or organize recent/high-quality papers about river or stream DOM, DOC, dissolved carbon, carbon flux, EEM-PARAFAC, riverine carbon cycling, CO2 evasion, land-ocean carbon export, or carbon-change mechanisms.
---

# River DOM Carbon Literature

## Core Rule

Do not answer from memory alone. For any "latest", "recent", "past N years", or "high-quality journal" request, browse and verify current bibliographic details before listing papers.

## Scope

Use for literature tasks involving:
- river, stream, fluvial, watershed, land-ocean aquatic continuum, estuary only when river export is central
- DOM, DOC, DIC, CDOM, FDOM, EEM-PARAFAC, dissolved carbon, organic carbon, carbon flux, CO2/CH4 evasion, carbon age, carbon transformation
- paper retrieval, screening, Chinese summaries, manuscript-facing reference selection

Do not use for generic ocean/lake/soil DOM unless the user broadens scope or the paper is directly about river-to-coast transfer.

## Search Workflow

1. Set the time window explicitly.
   - "最近十年" means from today's date minus 10 years through today.
   - "最新" means verify current year and recent online-first papers.
2. Build search queries from object + process + method.
   - See `references/query-patterns.md` for reusable query templates.
3. Screen each candidate before inclusion:
   - peer-reviewed journal article, not preprint/news/thesis
   - study object includes rivers/streams/fluvial networks or river export
   - method or variable actually matches the user scope
   - journal is high-quality or field-respected
   - title, year, journal, DOI/source link are cross-checked
   - every retained paper has a DOI or stable source URL before it appears in the final answer
4. Exclude weak matches:
   - lake-only, marine-only, soil-only, wastewater-only without river connection
   - articles that only mention DOM/DOC in background
   - preprints unless the user explicitly allows them
   - low-confidence or non-peer-reviewed sources
5. State evidence depth:
   - "based on journal page/abstract" for screening summaries
   - "full-text checked" only after opening full text and verifying methods/results

## Quality Filter

Prioritize these venues when relevant:
- Nature, Science, PNAS, Nature Geoscience, Nature Communications, Communications Earth & Environment
- Water Research, Environmental Science & Technology, Global Biogeochemical Cycles, Geophysical Research Letters, Global Change Biology
- Biogeosciences, Limnology and Oceanography, Limnology and Oceanography Letters, Journal of Hydrology
- Science of The Total Environment, Journal of Hazardous Materials, Catena, Earth-Science Reviews

High quality is not impact factor alone. Prefer papers with strong design, broad relevance, robust datasets, mechanistic clarity, or strong synthesis value.

## Output Templates

For a retrieval list, use:

| Direction | Paper | Journal/Year | DOI/Link | Why It Matters |
|---|---|---|---|---|

Hard rule: every paper row must include a DOI link or source link in the `DOI/Link` column.

Use this DOI/link standard:
- Prefer DOI links in the form `https://doi.org/...`.
- If no DOI can be found, write `DOI: none found` and include a stable official/primary source URL, such as publisher, PubMed, Copernicus, Nature, ACS, Wiley, Elsevier, institutional repository, or official data/report page.
- Do not include a paper in the retained list if neither DOI nor stable source URL can be verified.
- If the link is from a secondary index only, label it as secondary and continue searching for a primary page before finalizing.

For paper-by-paper summaries, use the user's requested headings when provided. Default Chinese scaffold:

- 主题
- 内容
- 思路
- 方法
- 结论
- 对河流 DOM/碳循环研究的启发

For synthesis, group papers into conceptual families, for example:
- hydrology and event transport
- land use, urbanization, and wastewater
- river regulation and dams
- DOM transformation and reactivity
- carbon export and CO2/CH4 evasion
- old carbon, permafrost, and carbon age
- source-to-sea / land-ocean continuum

## Claim Discipline

Use conservative wording:
- "supports", "suggests", "is consistent with" for abstract-level evidence
- do not invent PARAFAC component labels, sample counts, statistics, or quantitative findings
- if exact methods/results matter for manuscript use, reopen the original paper and verify full text
- distinguish fact from inference
- never present a bibliography item without a DOI or link; traceability is part of the answer, not optional formatting

## Common Failure Modes

- Keyword trap: search hits mention DOM but study lakes/oceans/soil. Fix by checking study object.
- Method trap: paper mentions EEM/PARAFAC in references but does not use it. Fix by checking methods/highlights/abstract.
- Recency trap: "latest" results include accepted manuscripts, preprints, or future issue dates. Fix by checking journal page and DOI.
- Over-summary trap: one-line abstracts are too thin. Fix by using theme/content/logic/method/conclusion.
- Citation trap: a title is found through a secondary page only. Fix by opening DOI, publisher page, PubMed, Nature, Copernicus, Wiley, ACS, Elsevier, or institutional publication page.
- Traceability trap: a list of paper titles is returned without DOI/source links. Fix by adding a `DOI/Link` column and verifying every row before final response.

## Final Response

Keep the answer in Chinese by default for this user's research-literature tasks. Preserve English technical terms, journal titles, paper titles, DOI strings, model names, and method names.
