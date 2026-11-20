# Internet of Things: Public Scoreboard

## 1,000 open tools, one builder, all verifiable

Numbers as of November 16, 2026, updated November 20, 2026. Every figure on this page is regenerated from the program's own records, listed under Counting Rules below. The published count moves only on verified read back from the public surfaces, never on build counts.

## The three numbers that matter

| Measure | Count |
|---|---|
| Tools built | 1,013 |
| Tools parity validated | 1,013 |
| Tools published and verified live | 482 |

Built, validated, and published are three separate numbers on purpose. The gap between the first two and the third is the publish train's remaining work: 531 tools. On November 1, 2026, the verified count was 51. Publish waves 20 to 27 moved it to 393, and waves 28 and 29 plus a single unit publish moved it to 482. A further publish wave is in progress.

## Published, by surface

Each of the 482 published tools was verified on every surface below at its release closeout. The surfaces must agree with each other, or the tool does not count.

| Surface | Verified |
|---|---|
| GitHub source repository and release | 482 of 482 |
| npm package, latest equal to release version | 482 of 482 |
| GHCR container image, version and latest tags | 482 of 482 |
| MCP Registry entry, active and latest, npm plus OCI | 482 of 482 |
| Final verification pass | Passed, 482 of 482 |

Final verification is a Shipcheck verdict of GO. Where Shipcheck itself could not render a verdict for a network reason, an independent verify-published ALL PASS read back on every surface closed the unit instead. Wave 27 closed 11 units that second way. Waves 28 and 29 and the single unit publish that followed closed all 89 of their units with a Shipcheck verdict of GO.

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
| External pull requests authored into other projects | 193 (61 merged, 101 open, 31 closed unmerged) | November 15, 2026 |

## Excluded and held, stated openly

- 1 build (beytsearch) was invalidated for a fabricated source spec. It is excluded from every count on this page and will never publish.
- 10 reserve builds held at the 1,000 freeze were built in the factory shape and counted in on November 2, 2026. They are part of the 1,013 built and validated total.
- Program goal line was 1,000 tools. The build program froze at 1,003 counted builds on October 30, 2026; the three builds past the line were completed batches in flight, verified like the rest, and stand counted. The 10 reserve builds were counted in on November 2, 2026, for 1,013 counted builds. No further build batches are running; publishing catch up is the active work.

## Counting rules, in plain words

1. Built means a complete tool exists in the program's records with its full factory file set.
2. Parity validated means an automated comparison confirmed the rebuild's tool interface matches its reference specification, and its test suite passed in a foreground verification run. Figures come from the verification runs themselves, never from a builder's summary.
3. Published means the full release pipeline finished (repository, tag and release, npm, container image, registry) and every surface was read back from the public internet and found in agreement, with a Shipcheck verdict of GO.
4. A read back that times out is recorded as unverified and rechecked. It is never counted as published and never reported as a failure.
5. Downloads cover live packages only. A package whose download read fails is excluded from the total, never counted as zero.

## Where each figure comes from

- Built and parity validated: the rebuild program scoreboard and build records (~/workspace/mcp-rebuild-100/SCOREBOARD.md, totals after reserve builds, November 2, 2026, and census after the linkledger single unit publish, November 16, 2026).
- Published and per surface verification: the publish train closeout records (~/workspace/mcp-rebuild-100/PUBLISH-WAVES.md, Wave 29 closeout and linkledger single unit closeout, November 16, 2026).
- Catalog: the ProdForge directory staging count recorded at the November 1, 2026 closeout.
- npm liveness and downloads: the fleet traction report generated November 1, 2026 (TRACTION.md).
- Policy index: the live Greenlight index totals (updated October 30, 2026) and the scan state file (November 1, 2026).
- Incident register: ~/workspace/security-wave/INJECTION-INCIDENTS.md, running totals after INC-043.
- Pull request census: the campaign census verified through the API on November 15, 2026, external projects only.

This page is regenerated from the program's own records, listed above, and the as of line is refreshed with each regeneration.
