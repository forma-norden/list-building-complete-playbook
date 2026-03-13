# list-data-validation-hygiene

Use this skill to protect your sending domains from burning. High bounce
rates are the #1 killer of outbound pipelines.

## The ZeroBounce Rule
Never, under any circumstances, send an aggressive cold email to an unverified email address.

## The Email Verification Waterfall
1. **Source Export:** Apollo / ZoomInfo exporting "Verified" status. (Usually 80-90% accurate).
2. **Dedicated Verifier:** Run the list through an API-focused verification tool (e.g., MillionVerifier, NeverBounce, ZeroBounce, or Reoon).
3. **The Catch-All Dilemma:** What do you do with "Catch-All" or "Accept-All" domains? 
   - *Strict Rule:* Throw them out. 
   - *Aggressive Rule:* Run them through a secondary catch-all verification tool like Scrubby.io. Do not send to them blindly.

## Data Decay and the 90-Day Rule
B2B contact data decays at a massive rate (people change jobs constantly).
- A verified list built today is safe to email tomorrow.
- A verified list built 60 days ago is risky.
- **A 90-day-old list must be entirely re-verified before being sequenced.**

## Cleaning the CRM "Gunk"
CRMs become graveyards of dead data.
- **Bounce Feedback Loop:** If an email bounces from an active sequence, you must automate a process to mark that contact as "Invalid" or "Bounced" in your CRM immediately. Do not rely on reps to do it manually.
- **The Semi-Annual Purge:** Twice a year, run your entire CRM contact database through a verifier and delete the hard bounces. This saves database costs and cleans up your reporting.

## Output Contract
When advising on data validation, provide:
- The recommended verification tool stack (Primary + Catch-all handling).
- The strict rules of engagement regarding Catch-All domains based on their risk tolerance.
- Instructions for setting up the bounce feedback loop from sequencer to CRM.
