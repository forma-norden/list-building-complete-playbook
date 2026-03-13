# Account Qualification Workflow

A checklist format to standardize how an SDR or automated system qualifies a raw list of accounts into the CRM.

## Phase 1: Firmographic Verification (The Baseline)
_Condition: If ANY step fails, disqualify the account entirely._

- [ ]  **Headcount Check:** Does the employee count fall within our defined ICP band? (e.g., 50-500 employees).
- [ ]  **Industry Check:** Is the primary industry explicitly supported by our platform?
- [ ]  **HQ Location Check:** Is the company headquartered in a region our legal/support teams can service?
- [ ]  **Business Model Check:** Are they B2B? (If we only sell B2B, disqualify B2C businesses regardless of size).

## Phase 2: Technographic & Competitive Check (The Environment)
_Condition: Depending on the product, this heavily impacts scoring or disqualifies._

- [ ]  **Required Tech:** Do they have the necessary prerequisite software installed? (e.g., Do they use Salesforce?)
- [ ]  **Competitor Check:** Are they currently locked into a known competitor contract? (If Yes, shift account to long-term "renewal nurture" status, do not run standard cold play).

## Phase 3: Buying Committee Mapping (The People)
_Condition: You must find these specific personas before launching the play._

- [ ]  **Identify The Budget Holder (Above the Line):** Find the VP or C-Level owner of the department. (Requires 1-2 contacts).
- [ ]  **Identify The Champion (Below the Line):** Find the Manager or Director who suffers the daily pain. (Requires 2-4 contacts).
- [ ]  **Verify Contact Data:** Run all identified emails through ZeroBounce/MillionVerifier. Ensure < 2% total list bounce rate.

## Phase 4: Signal Application (The Timing)
_Condition: Determines the SLA and the specific message angle._

- [ ]  **Check for Tier 1 Signals (Immediate Pain):** (e.g., Recent executive hire, pricing page visit, funding).
- [ ]  **Check for Tier 2 Signals (Latent Pain):** (e.g., Hiring in specific dept, general company growth).
- [ ]  **Assign Campaign Strategy:** 
    - If Tier 1 Signal -> Route to Manual Deep Personalization Play.
    - If Tier 2 Signal -> Route to AI-Assisted Templated Play.
    - If No Signal -> Route to Broad Segmented Play.

## CRM Logistics Sign-Off
- [ ] Deduplication Check: Ensure none of these domains are currently in an active sequence.
- [ ] Deduplication Check: Ensure these are not existing active customers.
- [ ] Upload to CRM with custom fields mapped specifically for the chosen playbook.
