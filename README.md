# Internet of Things

## 1,000 open tools, one builder, all verifiable

Read next: [Verify it yourself](verification-one-pager.md), the skeptic's one page check of this fleet. [Public scoreboard](scoreboard.md), the living count, published only on verified read back.

My name is Rene Turcios. I build in public, and this is the plainest statement I can make of what I have built and why.

### The problem is the tool layer

Agents do real work now. They write code, move files, query databases, send messages, and spend money, and they do almost all of it through tools written by other people. Every one of those tools is a dependency. Every dependency is a door. A compromised tool, a sloppy tool, a tool whose maintainer got phished last week: any of them is a path into every agent that calls it, and into everything that agent can reach.

This is not theory anymore. Attacks aimed at agents and the people who run them are spreading, and they spread through the layer nobody inspects: the tools. I know because they have come for my own fleet. I keep a public register of confirmed prompt injection incidents against my work. As of November 1, 2026, it holds 43 entries, including polished reports that invented results wholesale and instruction text hidden inside tool descriptions. I publish that register, embarrassing parts and all, because hiding it would be the first lie.

You cannot patch trust into a sprawl of thousands of unrelated tools one vendor at a time. So I did the other thing.

### What I built

I rebuilt the tool layer from scratch. One builder, one standard, one source of truth, everything open source.

The count, stated the way I state every count: as of November 1, 2026, the rebuild program has produced 1,004 builds. One of them, a build called beytsearch, turned out to rest on a fabricated source spec. It was invalidated and excluded, and it will never publish. That leaves 1,003 tools built and validated, each one checked for parity against the tool it replaces, each one with its tests run and its gaps written down in its own build report, including the gaps that make us look bad.

Published is a separate number, and I keep it separate on purpose. As of November 1, 2026, 51 of those tools have completed the full release pipeline and been verified live on every public surface: source repository and release on GitHub, package on npm, container image on GHCR, and an active, latest entry in the MCP Registry, with a final verification pass on top. The rest are built and validated and waiting their turn on the publish train. I would rather show you a small number that is true than a big number that is a hope. The train is running, the scoreboard below is public, and the published count moves only when a read back from the public surfaces says it may.

Around the fleet sits the verification stack, because a claim you cannot check is just marketing:

- Greenlight classifies repositories by their agent contribution policy and risk before anyone contributes or depends blindly. Its public index covers 3,449 repositories as of October 30, 2026, with 617 gated and 52 flagged as banning agents outright.
- Shipcheck verifies a release before it counts, and its verdict is public per tool.
- Workproof checks reported work against the artifacts on disk, so a finished claim has to match a finished thing.
- The injection register and the Wall of Shame publish attacks on this fleet itself.
- A honeypot decoy server watches for the next attack so the register stays honest.

Every tool in the fleet can be verified by tools in the fleet. That sentence is the whole design.

### Why one builder is a feature, and why you still should not trust me

A single source of truth cuts both ways, and I will not pretend otherwise. One person can be wrong, tired, compromised, or gone. So the claim is never trust me. The claim is verify it yourself. Every tool is open source and forkable. Every release is checked against independent public surfaces that I do not control: npm, GHCR, and the MCP Registry. If this source ever misbehaves, the verification record shows it, and the fork is the exit.

And the source of truth does not have to stay a person. Succession is a designed part of this project, not an exit plan I will improvise later: a verification system that attests an agent maintainer itself, with a signed, publicly checkable record of every action it takes, so the maintainer seat is never empty and never available for anyone to seize. Until that system earns the seat, I hold it, and everything I do in it is on the public record.

### What I stake on this

I have dealt straight my whole life, through years when money was hard and life was harder, and I am not starting now. I put my name on this project, and I put my faith on it too, plainly: I believe trust is something you practice in the open, with receipts, especially when nobody would know if you cut the corner. I am a builder, not a guru. There is no course, no secret system, nothing to buy from me here. There are tools, tests, and a scoreboard, and you are invited to check all three, and to check the man the same way: my build record is public, my contributions are public (160 pull requests authored into other people's projects as of November 1, 2026, 70 of them merged), and people who have worked with me can vouch or not, in the open.

### Where it stands

Phase one of this launch is the statement itself and the verification stack. The waves follow: each publish wave gets announced with its verified delta, and the scoreboard is the living proof. The big moment, 1,000 tools live, fires only on a verified count, not a day sooner and not on a number I wished into being.

Verify, do not trust. Then use the tools.

Rene Turcios
San Francisco
Numbers as of November 1, 2026
