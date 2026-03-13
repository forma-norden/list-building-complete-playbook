# list-company-sourcing

Use this skill to generate a list of target accounts (logos) that fit the
firmographic and technographic definitions of the ICP. Find the companies before you find the people.

## Top 4 Company Sourcing Methods

### 1. Database Filtering (Apollo / ZoomInfo)
- **Best for:** Broad firmographics (Industry, Headcount, Location).
- **Warning:** Employee headcount data is often lagged by 6-12 months. Startups that raised money 2 years ago might have 10 employees now, not 50.

### 2. Technographic Scraping (BuiltWith / HG Insights)
- **Best for:** Targeting companies based on their Web Stack (e.g., Shopify users, Stripe users).
- **Warning:** Does not catch internal SaaS tools (e.g., Slack vs Teams). Only catches what is embedded on the public-facing website.

### 3. Industry Directories (G2 / Capterra / Clutch)
- **Best for:** Identifying direct competitors or complementary providers.
- **Workflow:** Scrape a specific category (e.g., "Top SEO Agencies in London") using a tool like Clay or PhantomBuster. High accuracy, lower volume.

### 4. Job Board Scraping (Indeed / LinkedIn Jobs)
- **Best for:** Identifying companies with specific operational needs (Behavioral ICP).
- **Workflow:** Search for exact phrasing in JDs (e.g., companies requiring "Salesforce CPQ experience"). If they require the experience, they have the tool.

## The Account Waterfall Approach

Do not rely on one source for your Total Addressable Market (TAM).
1. Pull standard ICP from Apollo.
2. Cross-reference with BuiltWith data to filter out incompatible tech.
3. Layer on recent job post data to identify the top 10% most likely to buy.
4. Net result: A highly qualified list of accounts ready for contact discovery.

## Output Contract
When advising on company sourcing, provide:
- The optimal tool or combination of tools for their specific ICP constraints.
- Step-by-step search parameters (e.g., exact Apollo filters).
- The expected TAM size and how to narrow it down if it's too large (>2,000 accounts for a single campaign).
