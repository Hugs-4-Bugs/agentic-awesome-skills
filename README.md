<!-- registry-sync: version=7.2.0; skills=1232; stars=21535; updated_at=2026-03-08T08:00:03+00:00 -->
# 🌌 Agentic Awesome Skills: 1,232+ Agentic Skills for Claude Code, Gemini CLI, Cursor, Copilot & More

> **The Ultimate Collection of 1,232+ Universal Agentic Skills for AI Coding Assistants — Claude Code, Gemini CLI, Codex CLI, Antigravity IDE, GitHub Copilot, Cursor, OpenCode, AdaL**

[![GitHub stars](https://img.shields.io/badge/⭐%2021%2C000%2B%20Stars-gold?style=for-the-badge)](https://github.com/sickn33/antigravity-awesome-skills/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Anthropic-purple)](https://claude.ai)
[![Gemini CLI](https://img.shields.io/badge/Gemini%20CLI-Google-blue)](https://github.com/google-gemini/gemini-cli)
[![Codex CLI](https://img.shields.io/badge/Codex%20CLI-OpenAI-green)](https://github.com/openai/codex)
[![Kiro](https://img.shields.io/badge/Kiro-AWS-orange)](https://kiro.dev)
[![Cursor](https://img.shields.io/badge/Cursor-AI%20IDE-orange)](https://cursor.sh)
[![Copilot](https://img.shields.io/badge/GitHub%20Copilot-VSCode-lightblue)](https://github.com/features/copilot)
[![OpenCode](https://img.shields.io/badge/OpenCode-CLI-gray)](https://github.com/opencode-ai/opencode)
[![Antigravity](https://img.shields.io/badge/Antigravity-DeepMind-red)](https://github.com/sickn33/antigravity-awesome-skills)
[![AdaL CLI](https://img.shields.io/badge/AdaL%20CLI-SylphAI-pink)](https://sylph.ai/)
[![ASK Supported](https://img.shields.io/badge/ASK-Supported-blue)](https://github.com/yeasy/ask)
[![Web App](https://img.shields.io/badge/Web%20App-Browse%20Skills-blue)](apps/web-app)
[![Buy Me a Book](https://img.shields.io/badge/Buy%20me%20a-book-d13610?logo=buymeacoffee&logoColor=white)](https://buymeacoffee.com/sickn33)

**Antigravity Awesome Skills** is a curated, battle-tested library of **1,232+ high-performance agentic skills** designed to work seamlessly across the major AI coding assistants.

**Welcome to the V7.2.0 Release!** This repository gives your agent reusable playbooks for planning, coding, debugging, testing, security review, infrastructure work, product thinking, and much more.

## Table of Contents

- [🚀 New Here? Start Here!](#new-here-start-here)
- [📖 Complete Usage Guide](docs/users/usage.md) - **Start here if confused after installation!**
- [🔌 Compatibility & Invocation](#compatibility--invocation)
- [🛠️ Installation](#installation)
- [🧯 Troubleshooting](#troubleshooting)
- [🎁 Curated Collections (Bundles)](#curated-collections)
- [🧭 Antigravity Workflows](#antigravity-workflows)
- [📦 Features & Categories](#features--categories)
- [📚 Browse 1,232+ Skills](#browse-1232-skills)
- [🤝 How to Contribute](#how-to-contribute)
- [💬 Community](#community)
- [☕ Support the Project](#support-the-project)
- [🏆 Credits & Sources](#credits--sources)
- [⚖️ License](#license)
- [🌟 Star History](#star-history)

---

## New Here? Start Here!

**Welcome to the V7.2.0 Interactive Web Edition.** This isn't just a list of scripts; it's a complete operating system for your AI Agent.

### 1. 🐣 Context: What is this?

**Antigravity Awesome Skills** (Release 7.2.0) is a massive upgrade to your AI's capabilities.

AI Agents (like Claude Code, Cursor, or Gemini) are smart, but they lack **specific tools**. They don't know your company's "Deployment Protocol" or the specific syntax for "AWS CloudFormation".
**Skills** are small markdown files that teach them how to do these specific tasks perfectly, every time.

### 2. ⚡️ Quick Start (1 minute)

Install once; then use Starter Packs in [docs/users/bundles.md](docs/users/bundles.md) to focus on your role.

1. **Install**:

   ```bash
   # Default: ~/.gemini/antigravity/skills (Antigravity global). Use --path for other locations.
   npx antigravity-awesome-skills
   ```

2. **Verify**:

   ```bash
   test -d ~/.gemini/antigravity/skills && echo "Skills installed in ~/.gemini/antigravity/skills"
   ```

3. **Run your first skill**:

   > "Use **@brainstorming** to plan a SaaS MVP."

4. **Pick a bundle**:
   - **Web Dev?** start with `Web Wizard`.
   - **Security?** start with `Security Engineer`.
   - **General use?** start with `Essentials`.

### 3. 🧠 How to use

Once installed, just ask your agent naturally:

> "Use the **@brainstorming** skill to help me plan a SaaS."
> "Run **@lint-and-validate** on this file."

👉 **NEW:** [**Complete Usage Guide - Read This First!**](docs/users/usage.md) (answers: "What do I do after installation?", "How do I execute skills?", "What should prompts look like?")

👉 **[Full Getting Started Guide](docs/users/getting-started.md)**

---

## Compatibility & Invocation

These skills follow the universal **SKILL.md** format and work with any AI coding assistant that supports agentic skills.

| Tool            | Type | Invocation Example                | Path                                                                  |
| :-------------- | :--- | :-------------------------------- | :-------------------------------------------------------------------- |
| **Claude Code** | CLI  | `>> /skill-name help me...`       | `.claude/skills/`                                                     |
| **Gemini CLI**  | CLI  | `(User Prompt) Use skill-name...` | `.gemini/skills/`                                                     |
| **Codex CLI**   | CLI  | `(User Prompt) Use skill-name...` | `.codex/skills/`                                                      |
| **Kiro CLI**    | CLI  | `(Auto) Skills load on-demand`    | Global: `~/.kiro/skills/` · Workspace: `.kiro/skills/`                |
| **Kiro IDE**    | IDE  | `/skill-name or (Auto)`           | Global: `~/.kiro/skills/` · Workspace: `.kiro/skills/`                |
| **Antigravity** | IDE  | `(Agent Mode) Use skill...`       | Global: `~/.gemini/antigravity/skills/` · Workspace: `.agent/skills/` |
| **Cursor**      | IDE  | `@skill-name (in Chat)`           | `.cursor/skills/`                                                     |
| **Copilot**     | Ext  | `(Paste content manually)`        | N/A                                                                   |
| **OpenCode**    | CLI  | `opencode run @skill-name`        | `.agents/skills/`                                                     |
| **AdaL CLI**    | CLI  | `(Auto) Skills load on-demand`    | `.adal/skills/`                                                       |

> [!TIP]
> **Default installer path**: `~/.gemini/antigravity/skills` (Antigravity global). Use `--path ~/.agent/skills` for workspace-specific install. For manual clone, `.agent/skills/` works as workspace path for Antigravity.
> **OpenCode Path Update**: opencode path is changed to `.agents/skills` for global skills. See [Place Files](https://opencode.ai/docs/skills/#place-files) directive on OpenCode Docs.

> [!WARNING]
> **Windows Users**: this repository uses **symlinks** for official skills.
> See [Troubleshooting](#troubleshooting) for the exact fix.

---

## Installation

To use these skills with **Claude Code**, **Gemini CLI**, **Codex CLI**, **Kiro CLI**, **Kiro IDE**, **Cursor**, **Antigravity**, **OpenCode**, or **AdaL**:

### Option A: npx (recommended)

```bash
npx antigravity-awesome-skills
```

2. Verify the default install:

```bash
test -d ~/.gemini/antigravity/skills && echo "Skills installed"
```

3. Use your first skill:

```text
Use @brainstorming to plan a SaaS MVP.
```

4. Browse starter collections in [`docs/users/bundles.md`](docs/users/bundles.md) and execution playbooks in [`docs/users/workflows.md`](docs/users/workflows.md).

## Choose Your Tool

| Tool           | Install                                                | First Use                                            |
| -------------- | ------------------------------------------------------ | ---------------------------------------------------- |
| Claude Code    | `npx antigravity-awesome-skills --claude`              | `>> /brainstorming help me plan a feature`           |
| Cursor         | `npx antigravity-awesome-skills --cursor`              | `@brainstorming help me plan a feature`              |
| Gemini CLI     | `npx antigravity-awesome-skills --gemini`              | `Use brainstorming to plan a feature`                |
| Codex CLI      | `npx antigravity-awesome-skills --codex`               | `Use brainstorming to plan a feature`                |
| Antigravity    | `npx antigravity-awesome-skills --antigravity`         | `Use @brainstorming to plan a feature`               |
| Kiro CLI       | `npx antigravity-awesome-skills --kiro`                | `Use brainstorming to plan a feature`                |
| Kiro IDE       | `npx antigravity-awesome-skills --path ~/.kiro/skills` | `Use @brainstorming to plan a feature`               |
| GitHub Copilot | _No installer — paste skills or rules manually_        | `Ask Copilot to use brainstorming to plan a feature` |
| OpenCode       | `npx antigravity-awesome-skills --path .agents/skills` | `opencode run @brainstorming help me plan a feature` |
| AdaL CLI       | `npx antigravity-awesome-skills --path .adal/skills`   | `Use brainstorming to plan a feature`                |
| Custom path    | `npx antigravity-awesome-skills --path ./my-skills`    | Depends on your tool                                 |

## What This Repo Includes

- **Skills library**: `skills/` contains the reusable `SKILL.md` collection.
- **Installer**: the npm CLI installs skills into the right directory for each tool.
- **Catalog**: [`CATALOG.md`](CATALOG.md), `skills_index.json`, and `data/` provide generated indexes.
- **Web app**: [`apps/web-app`](apps/web-app) gives you search, filters, rendering, and copy helpers.
- **Bundles**: [`docs/users/bundles.md`](docs/users/bundles.md) groups starter skills by role.
- **Workflows**: [`docs/users/workflows.md`](docs/users/workflows.md) gives step-by-step execution playbooks.

## Project Structure

| Path                 | Purpose                                                   |
| -------------------- | --------------------------------------------------------- |
| `skills/`            | The canonical skill library                               |
| `docs/users/`        | Getting started, usage, bundles, workflows, visual guides |
| `docs/contributors/` | Templates, anatomy, examples, quality bar, community docs |
| `docs/maintainers/`  | Release, audit, CI drift, metadata maintenance docs       |
| `docs/sources/`      | Attribution and licensing references                      |
| `apps/web-app/`      | Interactive browser for the skill catalog                 |
| `tools/`             | Installer, validators, generators, and support scripts    |
| `data/`              | Generated catalog, aliases, bundles, and workflows        |

## Top Starter Skills

- `@brainstorming` for planning before implementation.
- `@architecture` for system and component design.
- `@test-driven-development` for TDD-oriented work.
- `@doc-coauthoring` for structured documentation writing.
- `@lint-and-validate` for lightweight quality checks.
- `@create-pr` for packaging work into a clean pull request.
- `@debugging-strategies` for systematic troubleshooting.
- `@api-design-principles` for API shape and consistency.
- `@frontend-design` for UI and interaction quality.
- `@security-auditor` for security-focused reviews.

## Three Real Examples

```text
Use @brainstorming to turn this product idea into a concrete MVP plan.
```

```text
Use @security-auditor to review this API endpoint for auth and validation risks.
```

## Curated Collections

**Bundles** are curated groups of skills for a specific role or goal (for example: `Web Wizard`, `Security Engineer`, `OSS Maintainer`).

They help you avoid picking from 1,236+ skills one by one.

### ⚠️ Important: Bundles Are NOT Separate Installations!

**Common confusion:** "Do I need to install each bundle separately?"

**Answer: NO!** Here's what bundles actually are:

**What bundles ARE:**

- ✅ Recommended skill lists organized by role
- ✅ Curated starting points to help you decide what to use
- ✅ Time-saving shortcuts for discovering relevant skills

**What bundles are NOT:**

- ❌ Separate installations or downloads
- ❌ Different git commands
- ❌ Something you need to "activate"

### How to use bundles:

1. **Install the repository once** (you already have all skills)
2. **Browse bundles** in [docs/users/bundles.md](docs/users/bundles.md) to find your role
3. **Pick 3-5 skills** from that bundle to start using in your prompts
4. **Reference them in your conversations** with your AI (e.g., "Use @brainstorming...")

For detailed examples of how to actually use skills, see the [**Usage Guide**](docs/users/usage.md).

### Examples:

- Building a SaaS MVP: `Essentials` + `Full-Stack Developer` + `QA & Testing`.
- Hardening production: `Security Developer` + `DevOps & Cloud` + `Observability & Monitoring`.
- Shipping OSS changes: `Essentials` + `OSS Maintainer`.

## Antigravity Workflows

Bundles help you choose skills. Workflows help you execute them in order.

- Use bundles when you need curated recommendations by role.
- Use workflows when you need step-by-step execution for a concrete goal.

Start here:

- [docs/users/workflows.md](docs/users/workflows.md): human-readable playbooks.
- [data/workflows.json](data/workflows.json): machine-readable workflow metadata.

Initial workflows include:

- Ship a SaaS MVP
- Security Audit for a Web App
- Build an AI Agent System
- QA and Browser Automation (with optional `@go-playwright` support for Go stacks)

## Features & Categories

The repository is organized into specialized domains to transform your AI into an expert across the entire software development lifecycle:

| Category       | Focus                                              | Example skills                                                                  |
| :------------- | :------------------------------------------------- | :------------------------------------------------------------------------------ |
| Architecture   | System design, ADRs, C4, and scalable patterns     | `architecture`, `c4-context`, `senior-architect`                                |
| Business       | Growth, pricing, CRO, SEO, and go-to-market        | `copywriting`, `pricing-strategy`, `seo-audit`                                  |
| Data & AI      | LLM apps, RAG, agents, observability, analytics    | `rag-engineer`, `prompt-engineer`, `langgraph`                                  |
| Development    | Language mastery, framework patterns, code quality | `typescript-expert`, `python-patterns`, `react-patterns`                        |
| General        | Planning, docs, product ops, writing, guidelines   | `brainstorming`, `doc-coauthoring`, `writing-plans`                             |
| Infrastructure | DevOps, cloud, serverless, deployment, CI/CD       | `docker-expert`, `aws-serverless`, `vercel-deployment`                          |
| Security       | AppSec, pentesting, vuln analysis, compliance      | `api-security-best-practices`, `sql-injection-testing`, `vulnerability-scanner` |
| Testing        | TDD, test design, fixes, QA workflows              | `test-driven-development`, `testing-patterns`, `test-fixing`                    |
| Workflow       | Automation, orchestration, jobs, agents            | `workflow-automation`, `inngest`, `trigger-dev`                                 |

Counts change as new skills are added. For the current full registry, see [CATALOG.md](CATALOG.md).

## Browse 1,232+ Skills

- Open the interactive browser in [`apps/web-app`](apps/web-app).
- Read the full catalog in [`CATALOG.md`](CATALOG.md).
- Start with role-based bundles in [`docs/users/bundles.md`](docs/users/bundles.md).
- Follow outcome-driven workflows in [`docs/users/workflows.md`](docs/users/workflows.md).
- Use the onboarding guides in [`docs/users/getting-started.md`](docs/users/getting-started.md) and [`docs/users/usage.md`](docs/users/usage.md).

## Documentation

| For Users                                                        | For Contributors                                                           | For Maintainers                                                                      |
| ---------------------------------------------------------------- | -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| [`docs/users/getting-started.md`](docs/users/getting-started.md) | [`CONTRIBUTING.md`](CONTRIBUTING.md)                                       | [`docs/maintainers/release-process.md`](docs/maintainers/release-process.md)         |
| [`docs/users/usage.md`](docs/users/usage.md)                     | [`docs/contributors/skill-anatomy.md`](docs/contributors/skill-anatomy.md) | [`docs/maintainers/audit.md`](docs/maintainers/audit.md)                             |
| [`docs/users/faq.md`](docs/users/faq.md)                         | [`docs/contributors/quality-bar.md`](docs/contributors/quality-bar.md)     | [`docs/maintainers/ci-drift-fix.md`](docs/maintainers/ci-drift-fix.md)               |
| [`docs/users/visual-guide.md`](docs/users/visual-guide.md)       | [`docs/contributors/examples.md`](docs/contributors/examples.md)           | [`docs/maintainers/skills-update-guide.md`](docs/maintainers/skills-update-guide.md) · [`.github/MAINTENANCE.md`](.github/MAINTENANCE.md) |

## Web App

The web app is the fastest way to navigate a large repository like this.

**Run locally:**

```bash
npm run app:install
npm run app:dev
```

That will copy the generated skill index into `apps/web-app/public/skills.json`, mirror the current `skills/` tree into `apps/web-app/public/skills/`, and start the Vite development server.

**Hosted online:** The same app is available at [https://sickn33.github.io/antigravity-awesome-skills/](https://sickn33.github.io/antigravity-awesome-skills/) and is deployed automatically on every push to `main`. To enable it once: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

## Contributing

- Add new skills under `skills/<skill-name>/SKILL.md`.
- Follow the contributor guide in [`CONTRIBUTING.md`](CONTRIBUTING.md).
- Use the template in [`docs/contributors/skill-template.md`](docs/contributors/skill-template.md).
- Validate with `npm run validate` before opening a PR.

## Community

- [Discussions](https://github.com/sickn33/antigravity-awesome-skills/discussions) for questions and feedback.
- [Issues](https://github.com/sickn33/antigravity-awesome-skills/issues) for bugs and improvement requests.
- [`SECURITY.md`](SECURITY.md) for security reporting.

## Support the Project

Support is optional. The project stays free and open-source for everyone.

- [Buy me a book on Buy Me a Coffee](https://buymeacoffee.com/sickn33)
- Star the repository
- Open reproducible issues
- Contribute docs, fixes, and skills

---

## Credits & Sources

We stand on the shoulders of giants.

👉 **[View the Full Attribution Ledger](docs/sources/sources.md)**

Key contributors and sources include:

- **HackTricks**
- **OWASP**
- **Anthropic / OpenAI / Google**
- **The Open Source Community**

This collection would not be possible without the incredible work of the Claude Code community and official sources:

### Official Sources

- **[anthropics/skills](https://github.com/anthropics/skills)**: Official Anthropic skills repository - Document manipulation (DOCX, PDF, PPTX, XLSX), Brand Guidelines, Internal Communications.
- **[anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks)**: Official notebooks and recipes for building with Claude.
- **[remotion-dev/skills](https://github.com/remotion-dev/skills)**: Official Remotion skills - Video creation in React with 28 modular rules.
- **[vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)**: Vercel Labs official skills - React Best Practices, Web Design Guidelines.
- **[openai/skills](https://github.com/openai/skills)**: OpenAI Codex skills catalog - Agent skills, Skill Creator, Concise Planning.
- **[supabase/agent-skills](https://github.com/supabase/agent-skills)**: Supabase official skills - Postgres Best Practices.
- **[microsoft/skills](https://github.com/microsoft/skills)**: Official Microsoft skills - Azure cloud services, Bot Framework, Cognitive Services, and enterprise development patterns across .NET, Python, TypeScript, Go, Rust, and Java.
- **[google-gemini/gemini-skills](https://github.com/google-gemini/gemini-skills)**: Official Gemini skills - Gemini API, SDK and model interactions.
- **[apify/agent-skills](https://github.com/apify/agent-skills)**: Official Apify skills - Web scraping, data extraction and automation.


### Inspirations

- **[f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)**: Inspiration for the Prompt Library.
- **[leonardomso/33-js-concepts](https://github.com/leonardomso/33-js-concepts)**: Inspiration for JavaScript Mastery.

### Additional Sources

- **[agent-cards/skill](https://github.com/agent-cards/skill)**: Manage prepaid virtual Visa cards for AI agents. Create cards, check balances, view credentials, close cards, and get support via MCP tools.

---

## License

MIT License. See [LICENSE](LICENSE) for details.

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=sickn33/antigravity-awesome-skills&type=date&legend=top-left)](https://www.star-history.com/#sickn33/antigravity-awesome-skills&type=date&legend=top-left)

If Antigravity Awesome Skills has been useful, consider ⭐ starring the repo!

<!-- GitHub Topics (for maintainers): claude-code, gemini-cli, codex-cli, antigravity, cursor, github-copilot, opencode, agentic-skills, ai-coding, llm-tools, ai-agents, autonomous-coding, mcp, ai-developer-tools, ai-pair-programming, vibe-coding, skill, skills, SKILL.md, rules.md, CLAUDE.md, GEMINI.md, CURSOR.md -->
