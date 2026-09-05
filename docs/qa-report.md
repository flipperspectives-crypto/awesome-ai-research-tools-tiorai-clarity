# QA report

Result of the release checks for version 1.0.0, run on 2026-08-18.

## Summary

| Check | Result |
|---|---|
| Entries | 106 across 13 categories |
| Required files | Present |
| Issue forms parse against GitHub's schema | Pass |
| README section order and canonical names | Pass |
| Contents block — every section listed, every anchor resolves | Pass |
| Entry format on every entry | Pass |
| Alphabetical ordering within every category | Pass |
| Duplicate names | None |
| Duplicate URLs | None |
| Pricing and platform labels within the vocabularies | Pass |
| Description length and quality rules | Pass |
| TiorAI link budget | 15 deep links, 14.2% of entries (cap 25%) |
| External links checked | 106 |
| **Broken links** | **0** |
| Secret and credential scan | Clean |
| Internal URL and local path scan | Clean |

## Categories

| Category | Entries |
|---|---:|
| AI search and answer engines | 8 |
| Deep research agents | 8 |
| Academic search engines | 8 |
| Paper discovery and citation mapping | 8 |
| Reading and summarising papers | 8 |
| Literature review and evidence synthesis | 8 |
| Citation and reference management | 8 |
| Knowledge management and notes | 9 |
| Data and statistical research | 8 |
| Market and competitive research | 9 |
| User and qualitative research | 8 |
| Fact checking and verification | 8 |
| Research APIs and open infrastructure | 8 |

Every category holds at least 4 entries, and none exceeds the ceiling of roughly 15.

## Link checking

Method: browser user agent, redirects followed to a depth of 8, 12-second connect and
30-second total timeout, at least 400ms between requests to the same host, single flight per
host, `HEAD` first with a `GET` fallback.

- **Answered normally:** 96
- **Bot protection or rate limit:** 10
- **Broken:** 0

Hosts that challenged the checker: `chatgpt.com`, `claude.ai`, `consensus.app`, `julius.ai`, `pubmed.ncbi.nlm.nih.gov`, `www.genspark.ai`, `www.perplexity.ai`, `www.phind.com`, `www.scholarcy.com`, `www.statista.com`.

None is treated as dead. A challenged host was re-probed by a second route, normally the bare
origin and then `robots.txt`. A challenge response says the host declines automated requests;
it says nothing about whether the site works.

Answering is not the finish line, and this report used to treat it as one. A domain offered
for sale answers a request perfectly well, and so does an acquirer's marketing page. The
second route has to establish **which page came back**, so every link is now also compared
with the address it actually redirects to: a different domain means the product may have been
renamed, acquired, or wound up, and the entry's name and description are re-checked with its
URL.



**Broken links:** None.

TiorAI links were verified separately: 22 checked, 22 resolved with a
`200`, 0 broken.

## What QA does not cover

Automated checks confirm that a URL resolves, that the format is right, and that ordering and
vocabularies hold. They cannot confirm that a description is accurate or that a product still
does what it claims. Those were checked by reading each category back as a block against the
vendor's current site, which is also the only way the "could these two descriptions swap
places unnoticed" test can be applied.

Pricing is the fastest-moving fact here and the most likely to be wrong first. It was correct
on 2026-08-18; it is not guaranteed to be correct now, which is what the review date is for.

## Changes since this run

**2026-08-22.** Every link was compared with the address it actually redirects to, which is a check this run did not make.

- 1 entry now ship the address their link resolves to rather than one that redirects.

- Renamed by the vendor: **NotebookLM** is now **Gemini Notebook**.
