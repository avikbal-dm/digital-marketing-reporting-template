# Claude prompt library

Copy-paste prompts to fill each tab of the reporting template with Claude and the Windsor.ai connector. Run them one at a time. Replace the angle-bracket placeholders with your account IDs the first time, then Claude remembers them for the rest of the session.

> Before you start: open Claude, turn on the **Windsor.ai** connector, and run the connect prompt to confirm your accounts.

## 0. Connect and confirm

> "Using the Windsor.ai connector, list the connectors and accounts I have connected. Confirm GA4, Search Console, Google Ads, and LinkedIn are available, and show me the account ID for each."

Note the IDs it returns. You will reuse them below.

## 1. KPI Monthly (the source of truth)

> "For my GA4 property `<GA4-ID>`, pull Total Users, engagement rate, bounce rate, and my lead key event by month for the last 6 months. Then pull organic clicks, impressions, and average position by month from Search Console for `<my domain>`. Then pull total paid spend by month from Google Ads `<ADS-ID>` and LinkedIn Ads `<LI-ID>`. Lay it out as one row per month matching the KPI Monthly columns, and leave any month where the lead event was not yet configured blank, not zero."

Fill the blue cells in KPI Monthly. The Executive Summary, Month-on-Month, and Quarterly tabs fill themselves.

## 2. By Channel

> "From GA4 `<GA4-ID>`, give me Total Users by default channel group by month for the last 6 months, plus my lead key event by channel for the latest month. Format it as a month-on-month matrix: channels in rows, each month split into Total Users and No. of Leads."

## 3. By Product

> "From GA4 `<GA4-ID>`, roll up Total Users, engagement rate, bounce rate, and leads by product section using the landing page path (group `/product-a*`, `/product-b*`, and so on) for the latest month. Add organic clicks, impressions, and average position per section from Search Console."

## 4. All Pages

> "From GA4 `<GA4-ID>`, list every landing page with 5+ sessions for the latest month with Total Users, engagement rate, bounce rate, and leads. Join organic clicks, impressions, and average position per page from Search Console. Sort by Total Users. Drop bot and probe paths."

## 5. Paid Campaigns

> "From Google Ads `<ADS-ID>` and LinkedIn Ads `<LI-ID>`, give me one row per campaign per month for the last 6 months: impressions, clicks, spend, and conversions. Tag each row with platform, channel, product, and geo."

## 6. SEO Keywords

> "From Search Console for `<my domain>`, list every query with at least one click for the last 6 months. For each, give the top ranking page (URL), total clicks, impressions, average position, and the first month it earned a click. Add a position band column (1-3, 4-10, 11-20, 21-50, 50+) and flag brand versus non-brand."

## 7. Page Speed

> "Run PageSpeed Insights (mobile) for my homepage and my top 10 pages. Return performance score, LCP, CLS, and FCP for each. If the public endpoint rate-limits, tell me and I will add a PSI API key."

## 8. AI Search

> "From GA4 `<GA4-ID>`, pull referral Total Users and leads from ChatGPT, Perplexity, and Gemini for the latest month, plus the AI Assistant channel total."

## 9. Geography

> "From GA4 `<GA4-ID>`, give Total Users and leads by country for the latest month, countries with 50+ users."

## 10. Write it into the workbook

> "Write all of this into my reporting workbook, filling the blue input cells on each tab. Keep every formula and the formatting intact. Do not change the structure."

## Tips

- Run tabs in order. KPI Monthly first, since the summary tabs depend on it.
- If a number looks off, ask Claude for the date range and filters it used, then check the Sources tab to match them.
- Keep the conversation open so Claude reuses your account IDs across prompts.
