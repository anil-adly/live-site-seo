# Live Site SEO

A reusable skill for **Codex and Claude Code** that audits already launched websites for Google organic traffic and AdSense readiness. Give it a URL; repository and Search Console access are optional.

It checks crawlability and indexing, keyword intent and long-tail opportunities, People Also Ask questions, titles, crawlable `href` links, canonicals, schema, performance, About/Contact/Privacy/Terms pages, ads, and measurement. It separates observed problems from unverified checks and protects existing useful URLs.

## Install in Codex

```sh
codex plugin marketplace add anil-adly/live-site-seo
codex plugin add live-site-seo@anil-adly-live-site-seo
```

Start a new task and ask:

```text
Use $live-site-seo to audit https://example.com for Google search traffic.
```

To install only the standalone skill, ask Codex's skill installer to install `plugins/live-site-seo/skills/live-site-seo` from this repository, or copy that folder into your personal Codex skills directory.

## Install in Claude Code

```sh
claude plugin marketplace add anil-adly/live-site-seo
claude plugin install live-site-seo@anil-adly-live-site-seo
```

Start a new session and run:

```text
/live-site-seo:live-site-seo https://example.com
```

For a standalone installation, copy `plugins/live-site-seo/skills/live-site-seo` to `~/.claude/skills/live-site-seo`; invoke it as `/live-site-seo`. Choose the plugin or standalone installation; you do not need both.

## Claude.ai and other chat apps

Download `live-site-seo.zip` from [Releases](https://github.com/anil-adly/live-site-seo/releases/latest) and upload it through your account's custom-skill settings where supported. A local Claude Code installation does not upload the skill to claude.ai. In chat apps without skill support, provide both `SKILL.md` and `references/checklist.md` as instructions.

This public repository is a community distribution. It is **not an approved listing in the OpenAI or Anthropic directories**. Directory publication uses their separate submission and review processes: [OpenAI](https://developers.openai.com/plugins/deploy/submission), [Anthropic](https://code.claude.com/docs/en/plugins/publish).

## Example requests

- Audit this launched site and prioritize the five fixes most likely to help organic traffic: https://example.com.
- Use Live Site SEO on this website and fix the confirmed issues in this repository.
- Check indexing, canonical URLs, schema, internal links, and policy pages only.
- Find long-tail opportunities for the existing tools before proposing new pages.

A URL-only request performs an audit. Ask explicitly for implementation or deployment when desired. The agent needs browsing/fetch tools for a live audit, and code access for implementation; it marks unavailable checks as unverified.

## What it avoids

No guaranteed rankings, keyword-difficulty-to-months promises, invented metrics, fabricated reviews, word-count quotas, automatic outreach, or mass low-value pages. It checks changing Google guidance at execution time. Reference guidance was reviewed on September 27, 2026.

## Contents

- [Skill instructions](plugins/live-site-seo/skills/live-site-seo/SKILL.md)
- [Detailed checklist and official sources](plugins/live-site-seo/skills/live-site-seo/references/checklist.md)

The package contains instructions only: no executable scripts, remote servers, credentials, or bundled telemetry. Your assistant and the tools you authorize determine which services receive data during use.

Report problems or suggestions in [Issues](https://github.com/anil-adly/live-site-seo/issues). MIT licensed; no affiliation with Google, OpenAI, or Anthropic.
