# Launched-site SEO and AdSense checks

Reference checked September 27, 2026. Verify current official requirements when using time-sensitive guidance. Apply these checks to the site's actual functionality and the user's requested scope.

## 1. Existing demand, competitors, and page targeting

Use existing Search Console data first when available: queries, pages, clicks, impressions, CTR, countries, devices, and comparable date ranges. Account for seasonality and changes in query mix. A `site:` search is not an exhaustive index report.

Research primary keywords, synonyms, long-tail queries, and relevant questions using available Ahrefs, Keyword Planner, Trends, autocomplete, People Also Ask, and related searches. Record source/date/market for observations. If those tools are unavailable, separate candidate ideas from verified metrics. Autocomplete is not a search-volume measurement.

Review actual leading pages for promising queries: intent, functionality, useful content, page-level links when available, and something our site can improve. Note widgets, AI Overviews, ads, and other features competing for clicks. Low DR, Reddit, or a weak-looking interface is a clue, not proof of easy rankings.

KD estimates difficulty reaching the top ten; it is not a time-to-rank formula. DR is not Google's own score. Google Ads competition/CPC is not organic difficulty or AdSense RPM. Do not add overlapping keyword volumes into projected visits. [Ahrefs methodology](https://ahrefs.com/keyword-difficulty).

Map related intent to the strongest existing URL before proposing new pages. Example: last name generator and random surname generator may share a page; a distinct elf-name tool may warrant another. Check competing site pages before merging; preserve useful content and redirect retired equivalents when justified. Recommend supporting guides only for real needs. Avoid doorway pages, fabricated locality, link schemes, and scaled low-value pages. [Google spam policies](https://developers.google.com/search/docs/essentials/spam-policies).

## 2. Crawlability, indexing, canonicals, and hosting

Inspect actual response status/headers, robots.txt, HTML robots directives, canonical tags, sitemap URLs, and redirects. Public pages intended for indexing should be accessible and return 200. Test a nonexistent URL for a real 404, and distinguish a genuine server error from a successful page.

Keep sitemaps limited to canonical, indexable URLs with truthful modification dates. Check that canonical, sitemap, internal links, and redirects agree. A sitemap assists discovery, not guaranteed inclusion.

An unintended production `X-Robots-Tag: noindex` is a blocker even when the page looks correct. A robots.txt crawl block does not reliably prevent indexing; Google needs access to discover noindex. Check both independently. Neither is private access control. [Noindex guidance](https://developers.google.com/search/docs/crawling-indexing/block-indexing).

Normalize equivalent protocol/host/slash variants appropriately. Do not flag a single intentional redirect as a major issue. Prefer permanent path-preserving redirects from redundant production hosting domains when feasible; audit host-specific noindex or authentication on previews separately. Never let preview restrictions spill onto the custom domain. Ordinary duplicate URLs are not automatically a penalty. [Canonical guidance](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls).

Inspect initial HTML and rendered content. Check crawlable links and access to rendering resources. Retain a working stack; static/server rendering can simplify discovery, but Astro, multi-page reloads, and framework migrations are not ranking requirements. [JavaScript SEO](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics).

## 3. Tool, content, metadata, and links

Test the main tool task with suitable non-sensitive input, realistic limits, error states, and output. Record what was actually tested. Keep the tool easy to reach; add clear instructions, original examples, method/limits, troubleshooting, and useful researched questions. Do not bury the tool beneath generic SEO prose.

Use original answers grounded in functionality. Claims such as accurate, private, lossless, unlimited, and no upload require evidence. No fixed 600-word quota, manufactured expertise, fake popularity, or cosmetic update dates. [Helpful-content guidance](https://developers.google.com/search/docs/fundamentals/creating-helpful-content).

Audit distinct titles/descriptions, a clear main heading, meaningful heading structure, readable URLs, relevant image alternatives, favicon, and sharing previews. Character counts are preview heuristics. Meta descriptions and social previews are not ranking guarantees. Skip meta-keywords. No exact-match domain or .com requirement. [SEO starter guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide).

Check real navigation `<a href="/path/">` links, descriptive anchors, orphan pages, broken destinations, redirect chains, and contextual links among tools/guides. Use buttons for actions. `href="#"` and click handlers are not substitutes for crawlable page links. Use `rel="sponsored"` for paid links and `rel="ugc"` for user-generated links where applicable. [Link guidance](https://developers.google.com/search/docs/crawling-indexing/links-crawlable).

Distinguish **Ahrefs** research, HTML **href**, and **hreflang**. Use hreflang only for genuine language/region alternatives, with valid codes, reciprocal/self entries, and compatible canonical URLs. Do not manufacture US targeting through irrelevant locale markup.

## 4. Structured data

Inventory existing JSON-LD in source and rendered DOM. Text-only fetches may remove scripts; missing schema is unverified until inspected appropriately. Preserve valid markup and avoid duplicates from templates/plugins.

Select types by actual content: WebSite for identity, Organization/Person for the actual publisher, BreadcrumbList for applicable navigation, SoftwareApplication/WebApplication for appropriate tools, and Article for real articles. Not every page needs all types.

Use factual visible content, consistent URLs/identifiers, and no invented reviews, ratings, claims, or credentials. Separate Schema.org validity from Google rich-result eligibility. Validate with Schema.org Validator and Google's Rich Results Test where available; distinguish required errors from optional recommendations. Unsupported rich-result types are not inherently invalid Schema.org. [Google schema policies](https://developers.google.com/search/docs/appearance/structured-data/sd-policies).

Software-app rich-result requirements currently include name, price, and a rating or review. A free price alone is insufficient; never fabricate a review to qualify. [Current app requirements](https://developers.google.com/search/docs/appearance/structured-data/software-app).

Google discontinued FAQ rich results starting May 7, 2026. Keep useful visible FAQs, but do not add FAQPage solely for that discontinued feature or promise a ranking benefit. Existing valid FAQPage need not be deleted merely because Google no longer shows that result. Recheck support at execution time. [Official change log](https://developers.google.com/search/updates).

## 5. About, Contact, Privacy, and Terms

Check that these pages exist, are easily reachable, and contain real site-specific information. A 200 response verifies availability, not truthful contents or working contact delivery.

- About: actual operator, purpose, maintenance, and relevant experience.
- Contact: monitored address or working form; submission tests send messages, so follow the user's authorization.
- Privacy: actual file processing/upload, local storage, logs, retention, analytics, advertising, cookies, third parties, and user controls. Files staying local does not mean no analytics/ad data leaves the browser.
- Terms: actual service scope, acceptable use, output limitations, and ownership terms. Missing operator/jurisdiction facts require factual input, not fictional boilerplate.

Treat these as transparency and applicable-policy work, not four guaranteed ranking/approval switches. Google requires specific advertising privacy disclosures. A published privacy page alone does not implement consent or prove legal compliance. [AdSense required content](https://support.google.com/adsense/answer/1348695?hl=en).

## 6. Performance, accessibility, and ads

Test desktop and narrow-screen functionality, keyboard access, labels, focus, contrast, and errors. Check PageSpeed Insights and available field data. Good Core Web Vitals targets at the 75th percentile are LCP ≤2.5s, INP ≤200ms, CLS ≤0.1. Distinguish field results from lab estimates; absent field data is unverified, not failure. [Web Vitals](https://web.dev/articles/vitals).

Optimize the specific slow path, unnecessary JavaScript, images/fonts, and heavy processing. Reserve ad dimensions and recheck after ads load. Avoid stack rewrites solely for a Lighthouse score.

For AdSense, verify current site/account eligibility. Do not impose ten daily visitors, a universal site age, or an arbitrary number of articles/pages. Use real account-provided publisher IDs and ads.txt records. A public ads.txt file cannot prove account approval. [Eligibility](https://support.google.com/adsense/answer/9724?hl=en), [ads.txt](https://support.google.com/adsense/answer/12171612?hl=en).

Check consent by visitor region, including certified-CMP requirements where applicable; avoid claiming a banner alone proves compliance. [Consent requirements](https://support.google.com/adsense/answer/13554116?hl=en).

Keep ads separate from repeated clicks, tool controls, and downloads. Avoid accidental-click layouts, artificial reloads, or forced ad interactions. [Placement policies](https://support.google.com/adsense/answer/1346295?hl=en).

## 7. Measurement and sustainable growth

When access exists, inspect Search Console indexing/canonicals, sitemap processing, query/page performance, manual actions, and security issues. Otherwise list the exact account checks needed while completing the public audit. Submitting sitemaps or requesting indexing is an account action, not something an audit silently performs. [Search Console guidance](https://developers.google.com/search/docs/monitor-debug/search-console-start).

Verify analytics once per real navigation and track tool starts/completions or downloads as events. Do not collect private input values. Repeated Generate clicks are not automatically pageviews or new ad impressions. Measure organic visits, country/device mix, useful tool use, and actual page RPM after monetization. Label traffic/RPM revenue scenarios as assumptions.

Recommend relevant communities, resource pages, or creators for legitimate discovery and earned links; do not claim that social shares directly raise rankings. Draft outreach only unless sending was requested.

For broad audits, plan a 30-day discovery/functionality check, a 60-day review of observed queries and underperforming pages, and a 90-day decision about expansion. These are review dates, not ranking deadlines. Do not automatically create scheduled tasks.
