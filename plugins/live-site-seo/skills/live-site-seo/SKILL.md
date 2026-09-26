---
name: live-site-seo
description: "Use when the user asks to audit or improve Google search traffic, technical or on-page SEO, schema, or AdSense readiness for an already launched website, especially a free-tool site. Applies to requests such as check my live site's SEO or fix SEO on this deployed website; not a new-site build or paid Google Ads campaign."
---

# Live Site SEO

Improve an existing site's organic search opportunity without disrupting working pages. For free-tool sites, optimize for useful tool visits and sustainable AdSense earnings, not unrelated product cross-selling.

Example: `Use $live-site-seo on https://example.com and fix the issues in this repository.`

## Start from the live site

- Take the URL from the request or verified project context. Ask for it only if missing or ambiguous. Repository, Ahrefs, and Search Console access are optional; their absence must not block a public-site audit.
- A URL-only invocation means audit and recommendations. A fix request authorizes scoped implementation where code access exists. Preserve existing authorization for deployment; invoking this skill alone does not authorize publication, account changes, or outreach.
- Read existing project context. Identify the tool, audience, site language, monetization state, and any stated market. Label country assumptions and distinguish observed Google results from generic search results.
- Record the current deployment and evidence before editing. Inspect the homepage, important tools/landing pages, navigation, policy pages, robots.txt, sitemap, a missing URL, and relevant host variants. Cover small sites fully when practical; sample larger sites and state coverage.

## Inspect and prioritize

Use [references/checklist.md](references/checklist.md) for the relevant checks; a full audit covers every category, while a narrow request uses only applicable sections. Read source/headers and a real rendered browser page when available. Text extraction alone cannot establish missing schema or working functionality.

Browse current official guidance for changing schema support and AdSense rules. Mark inaccessible checks **Unverified**. Never invent metrics, rankings, private account findings, legal/business facts, or test results.

Prioritize functional/indexing blockers, then intent/content gaps and internal links, performance, and optional enhancements. Protect useful URLs and current search traffic. Prefer an evidenced improvement over framework migrations, domain changes, or mass page creation.

## When fixing

Trace the relevant template, routes, metadata, and hosting configuration before editing. Reuse existing implementations. Verify local changes with appropriate checks and browser inspection at desktop and narrow widths. After an authorized deployment, verify the production responses and pages separately. A local fix is not a verified live fix.

Missing ownership, contact, data-retention, publisher-ID, or jurisdiction facts stay listed as missing; do not publish invented policies or integrations. Continue unrelated fixes.

## Return a usable result

Lead with the largest opportunity or blocker and the next actions. Include:

- Findings table: URL/file, observed evidence, impact, exact fix, and status (**Pass / Fail / Not applicable / Unverified**).
- For growth audits: prioritized keyword-to-existing-page map, sourced questions/long-tail opportunities, and new pages only for distinct needs. Label proposed keywords separately from measured demand.
- Missing access/facts and precisely what they would verify.
- If requested: changes made, validation, and local versus deployed status.
- A short measurement plan using Search Console and tool completions; add 30/60/90-day reviews for broader growth work, without scheduling them automatically.

Scale the report to the request. Avoid generic scores, ranking promises, and repeating this checklist as findings.
