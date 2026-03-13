# list-contact-discovery

Use this skill to map the buying committee and extract verifiable email
addresses for the target accounts.

## Buying Committee Mapping

Never rely on a single persona title. Search for the *function*, not the specific title, using Boolean search.

### The Boolean Magic String
If you need the head of marketing, searching "Chief Marketing Officer" misses 70% of the market.
**Use:** `(Marketing OR Demand Gen OR Growth) AND (VP OR Vice President OR Head OR Director OR Chief OR CMO)`

### The 3-Tier Buying Committee
When extracting contacts for an account > 100 employees, you must find:
1. **Above The Line (The Budget Holder):** VP or C-Level. They sign the check.
2. **Below The Line (The Champion):** Director or Manager. They own the daily pain.
3. **The Blocker (The Technical Reviewer):** IT, RevOps, Legal, or InfoSec. They can kill the deal.

## Contact Extraction Best Practices

### 1. LinkedIn Sales Navigator (The Gold Standard)
- Export leads using tools like Evaboot, Skrapp, or PhantomBuster.
- **Pro-Tip:** Always filter out "Past" roles. LinkedIn search defaults to "Current OR Past", which leads to massive bounce rates. Check the "Current" box explicitly.

### 2. Apollo / ZoomInfo (The Volume Standard)
- Good coverage, but average data decay.
- **Pro-Tip:** Filter by "Email Status = Verified". Never export "Guessed" or "Awaiting Verification" emails unless you are pushing them through a secondary verification tool.

### 3. The Clay Waterfall (The Modern Standard)
Instead of relying on Apollo, use Clay to waterfall through providers:
- Step 1: Prospeo (High accuracy for LinkedIn profiles).
- Step 2: Dropcontact (Pattern matching).
- Step 3: Hunter.io / Apollo (Fallback).

## Output Contract
When asked how to find contacts, provide:
- A custom Boolean search string optimized for the requested persona.
- A 3-tier buying committee map (Executive, Champion, Blocker) based on their product.
- The recommended extraction workflow.
