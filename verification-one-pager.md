# Verify It Yourself: The Internet of Things Fleet in One Page

For the skeptic. Everything below can be checked from a laptop in an afternoon, using only public surfaces. Numbers as of November 1, 2026.

## The claim

1,003 tools built and parity validated. 51 of them published and verified live on every public surface. One builder. Everything open source.

## Where things live

- Source repositories: github.com/CloudCorpRecords, one public repository per tool.
- Packages: npm, under the @reneturcios scope for rebuilds and the original fleet names (greenlight, shipcheck, mcpaudit, mcpvet, and the rest).
- Container images: GHCR, one image per published tool, tagged with its version and latest.
- Registry: the official MCP Registry, namespace io.github.CloudCorpRecords, one active entry per published tool with both an npm package and an OCI image attached.
- Catalog: the ProdForge directory lists 158 servers, 76 of them from this fleet (25 original fleet tools plus the 51 verified published rebuilds).

## Pick any published tool and check it, five ways

1. Source: open its GitHub repository. The release tag matches the version everywhere else, and the build report in the repo lists what was tested and what is honestly not covered.
2. Tests: the test suite is in the repository. Run it. The counts in the build report should match what you see.
3. npm: the package page shows the same version as latest. The package carries its registry name, so the registry entry and the npm package point at each other.
4. GHCR: the image carries the label io.modelcontextprotocol.server.name with the tool's registry name, and tags for its version and latest.
5. MCP Registry: the entry reads active and latest, and names the same npm package and the same container image you just checked.

If any one of the five disagrees with the others, the tool does not count as published under our rules, and we want to hear about it.

## How the published count is computed

Read back only. A tool joins the published count when its release pipeline finishes and a person or a verification run has read every surface back from the public internet and found them in agreement: repository release present and not a draft, npm latest equal to the release version, GHCR tags present, registry entry active and latest, and a Shipcheck verdict of GO. Build counts never feed the published count. A timed out read back is recorded as unverified, never as published and never as failed; it gets checked again.

## What is NOT claimed yet

- 952 of the 1,003 validated tools are not yet published. They are built, tested, and parity checked, and their public claim today is exactly that and nothing more. The publish train works the queue in scoreboard order; the count on the scoreboard moves as waves verify.
- One build, beytsearch, was invalidated after its source spec proved fabricated. It is excluded from every count above and will never publish. It stays in the record because deleting it would be a lie of omission.
- Ten further candidate builds sit verdicted and held past the 1,000 freeze. They are not counted and not published.
- The original fleet has one deliberate exception: 36 of its 37 packages are live on npm; the remaining one is excluded from npm by design (a token wall), with its registry and container surfaces verified instead.
- Fleet traction, stated with its scope: 30,706 npm downloads in the 30 days ending November 1, 2026, across the 36 live original fleet packages only. Rebuild downloads are not folded into that figure.
- Parity means the rebuild matches its reference tool's interface, verified against documented or probed specs. Where a reference could not be run live, the build report says so. Parity is not a claim that every tool was exercised against a live production service.

## The standing invitation

Run Shipcheck or Greenlight against any tool in this fleet and publish what you find. The fleet's own incident register, 43 confirmed entries as of November 1, 2026, exists because we publish what attackers and our own tooling do to us. Outside verification is not a threat to this project. It is the project.
