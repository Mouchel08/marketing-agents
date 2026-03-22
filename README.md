# Marketing Agents

> 7 specialist AI marketing agents built on Claude — SEO, CRO, Content, Paid, Growth, Sales & Strategy

[![GitHub Pages](https://img.shields.io/badge/Dashboard-Live-brightgreen)](https://mouchel08.github.io/marketing-agents/dashboard/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-orange.svg)](CHANGELOG.md)

## 🚀 Live Dashboard

**[→ Open Marketing Team Dashboard](https://mouchel08.github.io/marketing-agents/dashboard/)**

Your 7 AI specialists in a visual control panel — click any agent to open Claude.ai with the right context pre-loaded.

---

## 🤖 The 7 Agents

| Agent | Slash Command | Skills |
|-------|--------------|--------|
| SEO & Content | `/marketing:seo` | seo-audit, ai-seo, site-architecture, programmatic-seo, schema-markup, content-strategy |
| CRO | `/marketing:cro` | page-cro, signup-flow-cro, onboarding-cro, form-cro, popup-cro, paywall-upgrade-cro |
| Content & Copy | `/marketing:content` | copywriting, copy-editing, cold-email, email-sequence, social-content |
| Paid & Measurement | `/marketing:paid` | paid-ads, ad-creative, ab-test-setup, analytics-tracking |
| Growth & Retention | `/marketing:growth` | referral-program, free-tool-strategy, churn-prevention, lead-magnets |
| Sales & GTM | `/marketing:sales` | revops, sales-enablement, launch-strategy, pricing-strategy, competitor-alternatives |
| Strategy | `/marketing:strategy` | marketing-ideas, marketing-psychology, product-marketing-context |

---

## 📁 Repository Structure

```
marketing-agents/
├── agents/                  # Claude Code agent definitions (7 agents)
│   ├── seo-content-agent.md
│   ├── cro-agent.md
│   ├── content-copy-agent.md
│   ├── paid-measurement-agent.md
│   ├── growth-retention-agent.md
│   ├── sales-gtm-agent.md
│   └── strategy-agent.md
├── commands/
│   └── marketing/           # Slash commands (/marketing:seo etc.)
│       ├── seo.md
│       ├── cro.md
│       ├── content.md
│       ├── paid.md
│       ├── growth.md
│       ├── sales.md
│       └── strategy.md
├── skills/                  # 33 marketing skill reference docs
│   ├── seo-audit.md
│   ├── ai-seo.md
│   └── ... (33 total)
├── dashboard/
│   └── index.html           # Visual team dashboard (GitHub Pages)
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
└── LICENSE
```

---

## ⚡ Quick Start

### Option 1: Dashboard (no setup needed)
Open the [live dashboard](https://mouchel08.github.io/marketing-agents/dashboard/) in any browser. Click **Chat →** on any agent card to start a conversation in Claude.ai.

### Option 2: Claude Code Plugin
Install the plugin into Claude Code so agents and slash commands are available in every project:

```bash
# Clone into Claude Code plugin directory
git clone https://github.com/Mouchel08/marketing-agents.git \
  ~/.claude/plugins/cache/marketingskills/marketing-agents/1.0.0

# Register the plugin (edit ~/.claude/plugins/installed_plugins.json)
```

Then restart Claude Code — you'll see `/marketing:seo`, `/marketing:cro`, etc. as slash commands.

### Option 3: Direct slash commands
Copy any `commands/marketing/*.md` file into your project's `.claude/commands/` directory.

---

## 🎯 How Agents Work

Each agent is a markdown file with a YAML frontmatter block that tells Claude Code when to auto-dispatch it. When you describe a task, Claude detects the right specialist and hands off automatically.

Example:
```
User: "my landing page isn't converting well"
→ Claude auto-dispatches cro-agent
→ CRO specialist runs page-cro + paywall-upgrade-cro frameworks
```

### Product Marketing Context
All agents check for a `.agents/product-marketing-context.md` file in your project. Create this once and every agent will use your business context automatically.

---

## 📚 Skills Reference

The `skills/` folder contains 33 individual skill docs — each one defines the framework, checklist, and output format for a specific marketing task.

**SEO (6):** seo-audit · ai-seo · site-architecture · programmatic-seo · schema-markup · content-strategy

**CRO (6):** page-cro · signup-flow-cro · onboarding-cro · form-cro · popup-cro · paywall-upgrade-cro

**Content (5):** copywriting · copy-editing · cold-email · email-sequence · social-content

**Paid (4):** paid-ads · ad-creative · ab-test-setup · analytics-tracking

**Growth (4):** referral-program · free-tool-strategy · churn-prevention · lead-magnets

**Sales (5):** revops · sales-enablement · launch-strategy · pricing-strategy · competitor-alternatives

**Strategy (3):** marketing-ideas · marketing-psychology · product-marketing-context

---

## 🛠 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) to add new agents, improve skill docs, or extend the dashboard.

---

## 📄 License

MIT — see [LICENSE](LICENSE).
