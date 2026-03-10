# claude-skills-founder

**Claude Code skills for startup founders.**
Product briefs, competitor analysis, pricing strategy, pitch decks, and GTM plans — from your terminal.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Skills](https://img.shields.io/badge/skills-12-blue.svg)](#whats-included)
[![Claude Code](https://img.shields.io/badge/Claude_Code-compatible-blueviolet.svg)](https://docs.anthropic.com/en/docs/claude-code)

---

Every Claude Code skills pack we could find is developer-focused — code review, git workflows, security audits. Nothing for the founder sitting in a repo at 2am, trying to figure out if their idea is worth building.

We built these skills at [Emotix](https://emotix.co?utm_source=github&utm_medium=oss&utm_campaign=claude-skills-founder) while running our own startup. They encode the frameworks, questions, and patterns we wish we had on day one.

---

## What's included

| Skill | Command | What it does |
|-------|---------|-------------|
| **Validate Idea** | `/validate-idea` | Stress-test your idea with hard questions before writing code |
| **Product Brief** | `/product-brief` | Generate a structured brief from a one-sentence idea |
| **Competitor Matrix** | `/competitor-matrix` | Build a competitive analysis with feature comparison |
| **Persona Gen** | `/persona-gen` | Create 3 detailed user personas with scoring |
| **MVP Scope** | `/mvp-scope` | Define what to build and — more importantly — what to cut |
| **Pricing Strategy** | `/pricing-strategy` | Design tiers, model, and unit economics |
| **Go-to-Market** | `/go-to-market` | Pre-launch, launch day, and 90-day growth plan |
| **Pitch Deck** | `/pitch-deck` | 12-slide deck outline with slide-by-slide content |
| **Fundraise Prep** | `/fundraise-prep` | Readiness assessment, investor targeting, timeline |
| **Landing Page** | `/landing-page` | Conversion-optimized copy, section by section |
| **User Interviews** | `/user-interviews` | Mom Test interview script with analysis framework |
| **Metrics Dashboard** | `/metrics-dashboard` | Define the 5 metrics that actually matter at your stage |
| **Email Sequence** | `/email-sequence` | Onboarding or re-engagement emails, ready to send |

Every skill takes natural language input and returns structured, actionable output — not generic advice.

---

## Install

### Option 1: Add to your project (recommended)

Copy the `commands/` directory into your project's `.claude/` folder:

```bash
# From your project root
git clone https://github.com/emotixco/claude-skills-founder.git /tmp/claude-skills-founder
cp -r /tmp/claude-skills-founder/commands/ .claude/commands/founder/
rm -rf /tmp/claude-skills-founder
```

Skills will be available as `/founder:product-brief`, `/founder:competitor-matrix`, etc.

### Option 2: Add globally (available in all projects)

```bash
git clone https://github.com/emotixco/claude-skills-founder.git /tmp/claude-skills-founder
cp -r /tmp/claude-skills-founder/commands/ ~/.claude/commands/founder/
rm -rf /tmp/claude-skills-founder
```

### Option 3: Clone and symlink

```bash
git clone https://github.com/emotixco/claude-skills-founder.git ~/claude-skills-founder
ln -s ~/claude-skills-founder/commands ~/.claude/commands/founder
```

This lets you `git pull` for updates.

---

## Usage

Open Claude Code in your terminal and type any skill command with your context:

```
/founder:validate-idea An AI tool that analyzes startup pitch decks and gives investor-perspective feedback
```

```
/founder:competitor-matrix Project management tools for solo founders (not teams)
```

```
/founder:pricing-strategy B2B SaaS for restaurant inventory management, targeting independent restaurants with 1-3 locations
```

```
/founder:pitch-deck Pre-seed raise, $500K, AI-powered competitor analysis for startup founders, 200 beta users, $2K MRR
```

Every skill accepts free-form text as input. Be as specific as possible — the more context you give, the better the output.

---

## Skill details

### /validate-idea

The first skill you should run. Scores your idea across 7 dimensions (problem severity, market size, willingness to pay, competition gap, distribution, timing, founder fit) and gives a verdict: build, pivot, or kill.

Includes 3 specific validation experiments you can run in under 2 weeks for under $200.

### /product-brief

Turns a one-sentence idea into a structured brief: problem statement, target audience with personas, value proposition, MVP features (exactly 5-7), success metrics with 90-day targets, risk assessment, and GTM snapshot.

### /competitor-matrix

Identifies 5-8 competitors and builds a feature comparison table. Finds positioning gaps no one is filling, ranks threats, and recommends a niche to own.

### /persona-gen

Creates 3 distinct personas with day-in-the-life narratives, direct quotes, current workarounds, and decision-making patterns. Includes a priority matrix showing which persona to build for first.

### /mvp-scope

Takes your feature wishlist and triages ruthlessly into Must Have / Should Have / Won't Have. Defines the critical user flow (signup to value in under 5 steps), recommends a tech stack, and estimates build time for a solo developer.

### /pricing-strategy

Evaluates 6 pricing models, designs 3 tiers with specific prices and features, checks unit economics, and applies pricing psychology (anchoring, decoy effect, annual framing). Includes launch vs. scale pricing and grandfathering policy.

### /go-to-market

Week-by-week launch plan: pre-launch audience building, launch day platform strategy (Product Hunt, HN, Reddit, Twitter/X, LinkedIn), and 90-day post-launch growth with channel prioritization and budget allocation for $0-$500/month.

### /pitch-deck

12-slide outline with exact content for each slide: title, problem, solution, demo, market size, traction, business model, competition, GTM, team, the ask, and closing. Plus appendix recommendations for Q&A backup slides.

### /fundraise-prep

Readiness scorecard, round sizing with recommended instrument (SAFE, note, or priced round), investor targeting with a 50-investor pipeline framework, materials checklist, and a 12-week fundraising timeline.

### /landing-page

Complete copy for every section: hero (headline, subhead, CTA), problem, solution, how it works, social proof, pricing preview, FAQ, and final CTA. Includes SEO metadata. Written for conversion, not cleverness.

### /user-interviews

Interview script following The Mom Test methodology — no leading questions, no hypotheticals. Includes screening criteria, warm-up questions, problem exploration, solution exploration, and a reaction phase. Plus an analysis framework for synthesizing 5-8 interviews.

### /metrics-dashboard

Defines exactly 5 metrics tailored to your stage (not 15 vanity metrics). Each metric has a definition, target, and specific action if it's below target. Includes a weekly review template, tracking tool recommendations, and investor-ready benchmarks.

### /email-sequence

5-7 emails for onboarding or re-engagement. Complete copy for each: subject line with A/B variant, preview text, body (under 150 words), and one CTA. Includes timing, segmentation setup, and performance benchmarks.

---

## Philosophy

These skills are built on a few principles:

**Specificity over generality.** "Post on social media" is not a tactic. "Post a Show HN with a title under 80 characters, linking to a live demo, on a Tuesday at 9am ET" is a tactic. Every skill forces specific, actionable output.

**Opinionated over balanced.** Generic advice is free and worthless. These skills take positions — "kill this feature," "this price is too low," "your idea has a fatal flaw." Founders need honest pushback, not encouragement.

**Brevity over completeness.** Every skill has a word limit. A 5,000-word product brief is not more useful than a 1,500-word one — it's just harder to act on.

**Frameworks over free-form.** Structured output (scorecards, matrices, checklists) is easier to compare, share with co-founders, and revisit in 3 months.

---

## Contributing

Have a skill idea? Open an issue or submit a PR.

**To add a new skill:**

1. Create a markdown file in `commands/`
2. Add YAML frontmatter with `description` and `argument-hint`
3. Write clear instructions with sections, rules, and output format
4. Keep the expected output under 2000 words
5. Test it with 3 different inputs to make sure it generalizes

We're looking for skills that fill genuine gaps in the founder workflow — not developer tools repackaged with startup vocabulary.

---

## License

MIT — use these however you want.

---

Built by the [Emotix](https://emotix.co?utm_source=github&utm_medium=oss&utm_campaign=claude-skills-founder) team. We build AI agents that turn startup ideas into research, analysis, and product briefs.
