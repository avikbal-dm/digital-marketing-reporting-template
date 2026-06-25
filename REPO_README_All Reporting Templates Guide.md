# Digital Marketing Reporting Template (Claude Data-Pull Ready)

**A free, formula-driven digital marketing reporting template for Excel that Claude fills for you.** Connect your data sources once, ask Claude to pull GA4, Google Search Console, Google Ads, LinkedIn, and PageSpeed, and get a clean, executive-ready marketing report in minutes. No manual exports. No broken formulas. Plug and play.

![License: MIT](https://img.shields.io/badge/License-MIT-22a06b.svg)
![Format: Excel xlsx](https://img.shields.io/badge/Format-Excel%20.xlsx-217346.svg)
![Made with Claude](https://img.shields.io/badge/Built%20for-Claude%20%2B%20Windsor.ai-5a3df0.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-22a06b.svg)
![No build needed](https://img.shields.io/badge/Setup-download%20%26%20go-22a06b.svg)

> One source of truth for your marketing numbers. Type once a month, or let Claude pull everything. The executive summary, month-on-month, and quarterly views recompute on their own.

---

## Why this template

Marketing teams rebuild the same report every month by hand. This **marketing report template** is built once. The structure, the formulas, the conditional formatting, and the plain-language metric definitions ship ready. You supply the data, or Claude does it for you with the Windsor.ai connector.

If you have searched for a **digital marketing report template Excel**, a **GA4 reporting template**, a **monthly marketing dashboard**, an **SEO report template**, or a **marketing KPI tracker**, this is a single workbook that covers all of it and stays consistent across every tab.

## Who it is for

- In-house marketers and growth leads who report to a CEO or board every month
- SEO and paid media specialists who want one workbook instead of five exports
- Agencies that need a repeatable, white-label client reporting system
- Founders who want a clear read on traffic, leads, and spend without a BI tool

## Choose a template

| Template | Tabs | Best for |
|---|---|---|
| **Full** (`MarketingCommandCenter_TEMPLATE.xlsx`) | 17 | Cross-channel reporting with a By Product breakdown |
| **Lite** (`MarketingCommandCenter_SIMPLE_TEMPLATE.xlsx`) | 16 | Single-product sites, blogs, and lean teams. No product split, just All Pages |
| **Google Ads** (`MarketingCommandCenter_GoogleAds_TEMPLATE.xlsx`) | 12 | A dedicated Google Ads report: campaigns, campaign type, device, search terms, budget pacing |
| **LinkedIn Ads** (`MarketingCommandCenter_LinkedInAds_TEMPLATE.xlsx`) | 13 | A dedicated LinkedIn Ads report: campaigns, campaign group, objective, engagement, budget pacing, with an in-file Instructions & Prompts tab |
| **SEO** (`MarketingCommandCenter_SEO_TEMPLATE.xlsx`) | 14 | A dedicated organic-search report: top pages, top keywords, position bands, striking distance, Core Web Vitals, backlinks, with an in-file Instructions & Prompts tab |

The Full and Lite versions cover all channels (GA4, Search Console, Google Ads, LinkedIn, PageSpeed). The Google Ads, LinkedIn Ads, and SEO versions are focused single-channel reports. The LinkedIn Ads and SEO templates carry their own Instructions & Prompts tab inside the file, so you do not need to leave the workbook to fill them. All share the same green theme, formula-driven design, and Claude prompts.

## Table of contents

- [Features](#features)
- [What is inside](#what-is-inside)
- [Quick start](#quick-start)
- [Fill it with Claude (recommended)](#fill-it-with-claude-recommended)
- [Fill it by hand](#fill-it-by-hand)
- [Monthly refresh](#monthly-refresh)
- [Customizing](#customizing)
- [FAQ](#faq)
- [Keywords and topics](#keywords-and-topics)
- [License](#license)

## Features

- **17 ready-made tabs** covering traffic, leads, channels, campaigns, SEO keywords, page speed, AI search, geography, and risks
- **One volume metric everywhere: Total Users.** No mixing sessions in one tab and users in another, so your numbers reconcile
- **Type once, recompute everywhere.** Fill KPI Monthly and the summary, month-on-month, and quarterly tabs update on their own
- **Claude data-pull ready.** Copy-paste prompts pull every source through the Windsor.ai connector
- **Plain-language definitions** on every metric, written for a CEO with no marketing background
- **Source-verifiable.** A Sources tab links each number back to the tool that produced it
- **No build, no install, no subscription.** Download the `.xlsx` and go

## What is inside

The workbook has 17 tabs. You only ever type into one of them: KPI Monthly.

| Tab | What it shows |
|---|---|
| Guide | How to use the workbook and read the colors |
| Executive Summary | One-screen scorecard with a month dropdown |
| KPI Monthly | One row per month. The single source of truth |
| Month-on-Month | Percent change versus the prior month |
| Quarterly | Quarter-on-quarter rollup |
| By Product | Performance grouped by product or business line |
| All Pages | Per-page performance, every URL with traffic |
| By Channel | Total Users and leads by channel, month on month |
| Paid Campaigns | One row per campaign per month |
| SEO Keywords | Every ranking term with URL, position band, and clicks |
| Page Speed | Core Web Vitals per page |
| AI Search | Referral traffic from ChatGPT, Perplexity, Gemini |
| AI Prompt Coverage | A checklist to verify your AI search visibility |
| Risks & Fixes | Data-driven issues and the action for each |
| Geography | Total Users and leads by country |
| Definitions | Plain-language meaning of every metric |
| Sources | Every tool, account, and link to verify a number |

### Conventions

- **Blue cells are inputs. Grey and black cells are formulas.** Leave the formulas alone.
- **Percentages are stored as values.** 26.0% is held as 0.26.
- **Conversion rate is leads divided by Total Users**, the same way on every tab.

## Quick start

1. Download the version you want:
   - Full (17 tabs): [`template/MarketingCommandCenter_TEMPLATE.xlsx`](template/MarketingCommandCenter_TEMPLATE.xlsx)
   - Lite (16 tabs, no product split): [`template/MarketingCommandCenter_SIMPLE_TEMPLATE.xlsx`](template/MarketingCommandCenter_SIMPLE_TEMPLATE.xlsx)
   - Google Ads only (12 tabs): [`template/MarketingCommandCenter_GoogleAds_TEMPLATE.xlsx`](template/MarketingCommandCenter_GoogleAds_TEMPLATE.xlsx)
   - LinkedIn Ads only (13 tabs): [`template/MarketingCommandCenter_LinkedInAds_TEMPLATE.xlsx`](template/MarketingCommandCenter_LinkedInAds_TEMPLATE.xlsx)
   - SEO only (14 tabs): [`template/MarketingCommandCenter_SEO_TEMPLATE.xlsx`](template/MarketingCommandCenter_SEO_TEMPLATE.xlsx)
2. Open it and read the **Guide** tab.
3. Rename the sample products and brand to your own (see [Customizing](#customizing)).
4. Fill **KPI Monthly** by hand, or hand the job to Claude with the prompts below.

## Fill it with Claude (recommended)

This template is built to be filled by **Claude** using the **Windsor.ai** connector, which pipes 300+ marketing sources into one place so you do not need a separate integration per platform.

1. Open Claude and turn on the Windsor.ai connector.
2. Confirm your accounts are connected (GA4, Search Console, Google Ads, LinkedIn).
3. Work tab by tab using the prompt library: **[docs/PROMPTS.md](docs/PROMPTS.md)**.
4. Ask Claude to write the numbers straight into the workbook.

The full prompt for the source-of-truth tab looks like this:

> "For my GA4 property, pull Total Users, engagement rate, bounce rate, and my lead key event by month for the last 6 months. Then pull organic clicks, impressions, and average position by month from Search Console. Then pull total paid spend by month from Google Ads and LinkedIn Ads. Lay it out as one row per month matching the KPI Monthly columns, and leave any month where the lead event was not yet configured blank, not zero."

See **[docs/PROMPTS.md](docs/PROMPTS.md)** for the prompt that fills each of the other tabs.

## Fill it by hand

No Claude, no problem. Each tab maps to one source.

| Tab | Source | Key fields |
|---|---|---|
| KPI Monthly | GA4 + Search Console + Google Ads + LinkedIn | users, engagement, bounce, leads, spend, organic clicks/impr/position |
| By Channel | GA4 | channel group, total users, lead event (by month) |
| By Product | GA4 + Search Console | landing page section, users, engagement, bounce, leads, organic |
| All Pages | GA4 + Search Console | landing page, users, engagement, bounce, leads, organic |
| Paid Campaigns | Google Ads + LinkedIn Ads | campaign, month, impressions, clicks, spend, conversions |
| SEO Keywords | Search Console | query, page, clicks, impressions, position, month |
| Page Speed | PageSpeed Insights (PSI v5) | performance, LCP, CLS, FCP per URL |
| AI Search | GA4 | referral source, users, leads |
| Geography | GA4 | country, users, leads |

## Monthly refresh

When a month closes, you add one row. That is the whole job.

1. Open KPI Monthly. Find the new month row.
2. Fill the blue cells, or run the KPI Monthly prompt for that month.
3. Refresh the deep-dive tabs you care about.
4. Open Executive Summary and pick the new month from the dropdown.

## Customizing

- **Brand and domain:** edit the title on the Guide tab and the entries on the Sources tab. Replace the placeholder account IDs with yours.
- **Products:** the template ships with Product A, B, C. Rename them on By Product and in the Section column on All Pages.
- **Targets:** the workbook flags engagement, bounce, cost per lead, and CTR against default goals. Adjust them to re-baseline.

## FAQ

**Which version should I use, Full or Lite?**
Use Full if you report by product line or business unit, since it adds a By Product breakdown. Use Lite if you run a single-product site, a blog, or a lean setup. Lite drops the product split and reports at the page level on the All Pages tab. Everything else is identical.

**Which version should I use, Full, Lite, or Google Ads?**
Use Full for cross-channel reporting with a By Product breakdown. Use Lite for a single-product site or blog, where All Pages replaces the product split. Use the Google Ads template when you only need a PPC report: it goes deeper on campaigns, campaign type, device, search terms, and budget pacing, and skips the organic and channel tabs.

**Does the Google Ads template do budget pacing and ROAS?**
Yes. It has a Budget Pacing tab that projects month-end spend against your budget and flags Over, Under, or On track, plus ROAS, cost per conversion, conversion rate, and search impression share across the account, by campaign, by campaign type, and by device.

**Does the LinkedIn Ads template handle lead-gen forms?**
Yes, with one manual step. LinkedIn lead-gen form leads are not exposed by the data connector, so the template has a blue Leads column you fill from Campaign Manager or your CRM. Cost per lead and lead rate then calculate on their own. The template covers spend, CTR, CPC, CPM, engagement, conversions, and a breakdown by campaign, campaign group, and objective. Its full instructions and Claude prompts live on an Instructions & Prompts tab inside the file.

**What does the SEO template track?**
Organic clicks, impressions, CTR, and average position from Search Console, organic users and leads from GA4, ranking keywords, referring domains, and domain rating from Ahrefs, and Core Web Vitals from PageSpeed. It has dedicated tabs for top pages, top keywords, position bands, striking-distance keywords (the quick wins in positions 4 to 20), Core Web Vitals, and backlink growth. Its full instructions and Claude prompts live on an Instructions & Prompts tab inside the file.

**Is this digital marketing reporting template free?**
Yes. It is released under the MIT license. Use it, fork it, ship it, even in client work.

**Do I need Claude to use it?**
No. Claude plus Windsor.ai is the fast path, but you can fill every tab by hand from each platform's own export. The tab-to-source map shows what goes where.

**What data sources does it cover?**
Google Analytics 4 (GA4), Google Search Console, Google Ads, LinkedIn Ads and Organic, and PageSpeed Insights out of the box. Through Windsor.ai you can extend it to 300+ sources.

**Does it work in Google Sheets?**
Yes. Open the `.xlsx` in Google Sheets. The formulas and formatting carry over. For best results with the month dropdown, keep it in Excel.

**How is conversion rate calculated?**
Leads divided by Total Users, applied the same way on every tab so the numbers reconcile across the workbook.

**Why Total Users instead of sessions?**
Reports break trust when one tab shows sessions and another shows users. This template standardizes on Total Users everywhere.

**Can agencies use it for client reporting?**
Yes. Rename the brand, products, and sources per client and you have a repeatable white-label reporting system.

## Keywords and topics

Digital marketing report template, marketing reporting template Excel, monthly marketing report template, GA4 reporting template, Google Analytics 4 report, SEO report template, SEO reporting template Excel, organic search report, keyword ranking tracker, striking distance keywords, Core Web Vitals report, backlink report, marketing KPI dashboard, marketing dashboard Excel, paid media report, PPC report template, Google Ads report template, Google Ads dashboard Excel, ROAS tracker, budget pacing template, search terms report, LinkedIn Ads report, LinkedIn Ads report template, LinkedIn Ads dashboard, cost per lead tracker, Search Console report, Core Web Vitals report, AI search visibility, Claude marketing reporting, Windsor.ai, plug and play marketing reporting system, agency client reporting template.

## License

[MIT](LICENSE). Use it, fork it, ship it. Attribution welcome, not required.

---

If this saves you a reporting cycle, **star the repo** so more marketers find it.
