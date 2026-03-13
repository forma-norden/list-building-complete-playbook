# list-deduplication-merge

Use this skill to prevent the cardinal sin of SDR work: emailing the same
person twice, on the same day, from two different reps.

## The Chaos of Multi-Sourcing

When you extract data from Apollo, Clay, and LinkedIn concurrently, you will generate duplicates. You must have a strict deduplication hierarchy before uploading to your CRM or Sequencer.

## The Deduplication Keys

Do not trust "First Name + Last Name". There are many "John Smiths."
1. **Primary Key (Contacts):** `Email Address`. This is the only globally unique identifier.
2. **Primary Key (Accounts):** `Company Domain` (e.g., acme.com). Do not use the Company Name string ("Acme", "Acme Inc.", "Acme LLC" will fail).
3. **Secondary Key (LinkedIn):** `LinkedIn Profile URL`. Highly reliable across platforms.

## The "Master Record" Conflict

When merging two duplicate records, which data survives?
- **Hierarchy of Trust:**
  1. *CRM Data (User inputted):* Highest trust. If the AE updated the phone number yesterday, keep it.
  2. *Verified 3rd-Party Enrichment:* Medium trust. Overwrite blank fields.
  3. *Raw Scraped Data:* Lowest trust.

## The "Currently In Sequence" Check

Before uploading any new list, you must run it against your CRM/Sequencer checking for:
`Active Sequence Status = TRUE`
If you do not do this, you will double-sequence prospects.

## Output Contract
When advising on deduplication, provide:
- The specific mapping keys required for importing the CSV/JSON into their CRM.
- The recommended conflict resolution rules (which data wins).
- A checklist for validating that the list doesn't overlap with currently active sequences.
