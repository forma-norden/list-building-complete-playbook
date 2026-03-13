# list-account-qualification

Use this skill to score and rank a master list of target accounts. A list
of 1,000 companies should not be sequenced randomly.

## The Account Scoring Matrix (0-100 Points)

Assign points based on how closely an account matches the ideal state.

### 1. Firmographic Fit (0-40 Points)
- **Sweet Spot:** Exactly in the optimal revenue/headcount band (40 pts).
- **Edge ICP:** Slightly too small or large, but viable (20 pts).
- **Out of Bounds:** Wrong size or industry (0 pts -> Disqualify).

### 2. Signal / Intent Layer (0-40 Points)
- **High Intent:** Recent funding, key executive hire, pricing page visit (40 pts).
- **Medium Intent:** Hiring in relevant dept, tech stack match (25 pts).
- **Static:** No current active signals (0 pts).

### 3. Relationship Layer (0-20 Points)
- **Strong:** Closed-lost deal > 6 months ago, past champion works there (20 pts).
- **Weak:** Attended a webinar last year (10 pts).
- **Cold:** Zero prior contact (0 pts).

## Tier Assignment and Execution

Calculate the score and route the accounts to the appropriate GTM play.

| Score | Tier Assignment | Execution Strategy |
|-------|-----------------|--------------------|
| **80-100** | Tier 1 (Whales) | Route to Senior AE. Manual research. Deep multi-threading. Phone + Voice notes + Custom Video. |
| **50-79** | Tier 2 (Dolphins) | Route to SDRs. AI-assisted personalization. Trigger-based sequencing. |
| **20-49** | Tier 3 (Minnows) | Pure automation. Highly segmented, persona-based messaging. No manual touches. |
| **<20** | Disqualified | Do not sequence. Keep in CRM for future enrichment passes. |

## Lookalike Modeling

If you don't know your scoring weights, reverse-engineer your closed-won deals.
1. Export your last 20 closed-won customers.
2. Find their commonalities (e.g., 80% use Stripe, 60% raised Series A in the last year).
3. Weight those variables heavily in your matrix.

## Output Contract
When asked to qualify or score a list, provide:
- A custom scoring matrix based on the user's specific ICP and available data.
- The execution rules for Tiers 1, 2, and 3.
- Instructions on how to automate this scoring inside Clay or a CRM.
