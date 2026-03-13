# List Building Benchmarks

Expected data coverage, decay rates, and accuracy metrics. Use this to forecast data costs and predict sequence volume.

## Data Accuracy by Source Type

| Source Type | Initial Accuracy | Validation Required | Primary Risk |
|-------------|------------------|---------------------|--------------|
| Self-Reported (Sales Nav, Job Boards) | 90-95% | Yes (For Emails) | People inflate titles or leave old jobs active |
| Crowdsourced (ZoomInfo, Apollo databases)| 75-85% | Mandatory | Stale data, high bounce rates if unverified |
| Web Scraped (BuiltWith technographics)| 80-90% | No | False positives (old pixels left on site) |
| API Enriched (Clay, Clearbit) | 85-95% | Highly Recommended| API hallucination or mismatched company domains |

## The Data Decay Model

B2B data rots quickly. The larger the company, the faster the churn.

- **Monthly Decay Rate (General B2B):** ~2.5 - 3% per month.
- **Startup Sector Penalty (High Growth):** ~4 - 5% per month.
- **Enterprise Executive Penalty:** Lower churn for C-suite, extremely high churn for SDRs/Junior roles.

*The 90-Day Cliff:* Any list generated more than 90 days ago will experience an 8-10% natural bounce rate. It must be run through a Bulk Verifier again before sending.

## The Cost per Lead Matrix

Expected industry averages for acquiring verified B2B contact data.

- **Bulk Database Export (Apollo/ZoomInfo):** $0.10 - $0.50 per verified contact. (Requires expensive annual contract).
- **Waterfall Enrichment (Clay/n8n):** $0.15 - $0.35 per verified contact. (Highly accurate, pay-as-you-go).
- **Manual Deep Research (Upwork/Fiverr):** $0.50 - $1.50 per verified contact. (Required for niche industries).
- **Inbound Lead Gen (Content/Ads):** $50 - $250+ per lead. (Highest intent, highest cost).

## Verification Outcome Benchmarks

When running a raw scraped list through a verification tool (like MillionVerifier or ZeroBounce), expect the following breakdown:

| Status | Expected % of List | Action |
|--------|---------------------|--------|
| Valid/Verified | 60 - 70% | Safe to email. |
| Invalid/Bounced | 15 - 20% | Delete immediately. |
| Catch-All/Accept-All | 10 - 15% | Isolate. Do not send without secondary verification. |
| Unknown/Spam Trap | ~1% | Delete immediately. |
