# Internet of Things: Public Scoreboard

## 1,000 open tools, one builder, all verifiable

Numbers as of November 1, 2026, 12:15 PM Pacific. Every figure on this page is regenerated from the program's own records, listed under Counting Rules below. The published count moves only on verified read back from the public surfaces, never on build counts.

## The three numbers that matter

| Measure | Count |
|---|---|
| Tools built | 1,003 |
| Tools parity validated | 1,003 |
| Tools published and verified live | 51 |

Built, validated, and published are three separate numbers on purpose. The gap between the first two and the third is the publish train's remaining work: 952 tools.

## Published, by surface

Each of the 51 published tools was verified on every surface below at its release closeout. The surfaces must agree with each other, or the tool does not count.

| Surface | Verified |
|---|---|
| GitHub source repository and release | 51 of 51 |
| npm package, latest equal to release version | 51 of 51 |
| GHCR container image, version and latest tags | 51 of 51 |
| MCP Registry entry, active and latest, npm plus OCI | 51 of 51 |
| Shipcheck final verdict | GO, 51 of 51 |

## The wider fleet

| Measure | Count | As of |
|---|---|---|
| ProdForge catalog entries | 158 servers | November 1, 2026 |
| Catalog entries from this fleet | 76 (25 original tools plus 51 rebuilds) | November 1, 2026 |
| Original fleet packages live on npm | 36 of 37 (one excluded by design) | November 1, 2026 |
| npm downloads, original fleet, last 30 days | 30,706 | November 1, 2026 |
| Greenlight policy index, repositories classified | 3,449 (617 gated, 52 agents banned) | October 30, 2026 |
| Greenlight deep scan progress | 4,872 of 5,200 candidate repositories | November 1, 2026 |
| Public injection incident register | 43 confirmed incidents | November 1, 2026 |
| Pull requests authored into other projects | 160 (70 merged, 66 open, 24 closed unmerged) | November 1, 2026 |

## Excluded and held, stated openly

- 1 build (beytsearch) was invalidated for a fabricated source spec. It is excluded from every count on this page and will never publish.
- 10 candidate builds are verdicted and held past the 1,000 freeze. Not counted, not published.
- Program goal line was 1,000 tools. The build program froze at 1,003 counted builds on October 30, 2026; the three builds past the line were completed batches in flight, verified like the rest, and stand counted. No further build batches are running; publishing catch up is the active work.

## Counting rules, in plain words

1. Built means a complete tool exists in the program's records with its full factory file set.
2. Parity validated means an automated comparison confirmed the rebuild's tool interface matches its reference specification, and its test suite passed in a foreground verification run. Figures come from the verification runs themselves, never from a builder's summary.
3. Published means the full release pipeline finished (repository, tag and release, npm, container image, registry) and every surface was read back from the public internet and found in agreement, with a Shipcheck verdict of GO.
4. A read back that times out is recorded as unverified and rechecked. It is never counted as published and never reported as a failure.
5. Downloads cover live packages only. A package whose download read fails is excluded from the total, never counted as zero.

## Where each figure comes from

- Built and parity validated: the rebuild program scoreboard and build records (~/workspace/mcp-rebuild-100/SCOREBOARD.md, freeze addendum of October 30, 2026).
- Published and per surface verification: the publish train closeout records (PUBLISH-WAVES.md closeout and RAZER-SLICE-1-2026-10-31.md, November 1, 2026).
- Catalog: the ProdForge directory staging count recorded at the November 1, 2026 closeout.
- npm liveness and downloads: the fleet traction report generated November 1, 2026 (TRACTION.md).
- Policy index: the live Greenlight index totals (updated October 30, 2026) and the scan state file (November 1, 2026).
- Incident register: ~/workspace/security-wave/INJECTION-INCIDENTS.md, running totals after INC-043.
- Pull request census: the campaign census verified through the API on November 1, 2026.

This page is regenerated from the program's own records, listed above, and the as of line is refreshed with each regeneration.
