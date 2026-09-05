# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 310 |
| Shortlisted after scope filtering | 148 |
| **Published** | **106** |

## Why candidates were dropped

- **General chatbot, no research mode.** The largest exclusion, and the reason several
  well-known assistants do not appear.
- **Undocumented source grounding.** A number of products claim to cite sources without
  describing what corpus they search. Those were dropped rather than described vaguely.
- **AI-content detection.** Excluded as a category. It is marketed heavily to academics, its
  published accuracy does not support the decisions people make with it, and listing it beside
  fact checking would imply an equivalence that does not exist.
- **Essay and paper generation.** Out of scope on purpose.
- **Note apps with no research workflow.** They belong in `awesome-ai-productivity-tools`.
- **Dead or renamed products.** Several tools in this category shut down or were acquired
  during the build; those were removed rather than linked to a redirect.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 106 distinct external URLs were checked:
96 answered normally, 10 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
