<div align="center">

# 🤝 negotiation-coach

### Turn any AI agent into a negotiation coach that hands you the exact words to say.

Salary counters · job offers · freelance rates · vendor & price haggling · rent - powered by 10 proven psychological tactics, with **ready-to-send scripts**, not vague "just be confident" advice.

[![Validate Skill](https://github.com/HemanthGangula/negotiation-coach/actions/workflows/validate.yml/badge.svg)](https://github.com/HemanthGangula/negotiation-coach/actions/workflows/validate.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

**[Quickstart](#-quickstart-60-seconds) · [See it in action](#-see-it-in-action) · [The 10 tactics](#the-10-tactics) · [Install everywhere](#-install-everywhere) · [FAQ](#-faq)**

</div>

---

## ⚡ Quickstart (60 seconds)

```bash
npx skills add HemanthGangula/negotiation-coach
```

That's it. Works across Claude Code, Cursor, Codex CLI, Gemini CLI, Windsurf, and 30+ other agents that read the open [`SKILL.md`](https://agentskills.io) format. Now just describe your situation:

> *"They offered me $95k, I wanted $110k, and I have no competing offer. Help me counter."*

The skill takes it from there. Prefer to install by hand or use Claude.ai? → [Install everywhere](#-install-everywhere).

---

## 🎬 See it in action

Here's the difference between a generic chatbot and this skill on the same prompt.

> **You:** They offered me $95k. I was hoping for $110k. I don't have another offer. What do I say?

<table>
<tr>
<td width="50%" valign="top">

**❌ Generic AI**

> Thanks for the offer! I was hoping for something closer to $110k. Is there any flexibility?

*Reveals your target, no leverage read, no plan, folds on the first "no."*

</td>
<td width="50%" valign="top">

**✅ negotiation-coach**

> **First, your BATNA is weak** (no competing offer) - so we don't bluff or ultimatum. We anchor once, then use silence and trading. Here's your counter:
>
> *"Thanks - I'm genuinely excited about the role. Based on the scope and market for this position, I was targeting $115k. Can we get there?"*
>
> Then **stop talking.** Let them respond first.
>
> ⚠️ *Anchor at $115k (above your $110k target), not your minimum - you'll get negotiated down. Don't justify the number; let the silence do the work.*

</td>
</tr>
</table>

You walk away with the literal sentence, *why* it works, and the way it can backfire - not a concept to go figure out yourself.

---

## Why this exists

Most people negotiate a handful of times a year - a salary, a rate, a lease, a big purchase. That's not enough reps to get good. The other side - a recruiter, a hiring manager, procurement, a landlord - often negotiates for a living. **This skill closes the gap:** a structured, repeatable coaching process instead of "just be confident," so you show up with an actual plan and actual words.

It ships as an open [Agent Skill](https://agentskills.io) - a portable, versioned, forkable folder, not a one-off prompt - so it works the same in whatever AI tool you already use.

## The 10 tactics

| Tactic | What it does |
|---|---|
| **⚓ Anchoring** | Sets the reference point by going first with a bold, credible number |
| **🪞 Mirroring** | Echoes their last few words as a question to draw out more information |
| **🤫 Tactical silence** | Uses the discomfort of a pause to make the other side fill the gap |
| **😬 The flinch** | A visible reaction of surprise that plants doubt about their number |
| **👮 Good cop / bad cop** | Recognizing (and ethically using) a real constraint as leverage |
| **🚪 Door-in-the-face** | Opens big to make the real ask look modest by contrast |
| **🅱️ BATNA** | Diagnoses your best alternative first - it decides how aggressive you can be |
| **🍪 The nibble** | One small extra ask after the deal is essentially agreed |
| **✋ The ultimatum** | A hard line, used only when you have real leverage to back it up |
| **🔄 Trading, not giving** | Never hands over a concession without asking for one in return |

Full breakdown of each - psychology, script, and failure mode - lives in [`references/tactics.md`](./references/tactics.md).

## What you can throw at it

<details>
<summary><b>💼 Salary & job offers</b></summary>

- *"I got an offer for $95k, I was hoping for $110k, and I don't have a competing offer. Help me counter."*
- *"They said 'this is the best we can do.' What do I say next?"*
- *"Help me figure out my BATNA before I negotiate next week."*
</details>

<details>
<summary><b>🧑‍💻 Freelance & contract rates</b></summary>

- *"A client wants my quote for a 3-month contract. I want to anchor high without scaring them off."*
- *"My client asked for a 20% discount. Help me trade instead of just saying yes."*
</details>

<details>
<summary><b>🛒 Vendor, price & purchases</b></summary>

- *"I'm buying a used car listed at $18,000. Walk me through how to open and where to land."*
- *"A SaaS vendor sent a renewal quote 30% higher than last year. Help me push back."*
</details>

<details>
<summary><b>🕵️ Spotting tactics used on YOU</b></summary>

- *"The recruiter keeps saying they need to check with the hiring manager on every number. Real constraint or a tactic?"*
- *"They went silent after my counter-offer. What's happening and what do I do?"*
</details>

<details>
<summary><b>🏠 Rent, lease & everyday bargaining</b></summary>

- *"My landlord wants a 10% rent increase. I want a smaller increase and a longer lease term. Help me script it."*
</details>

> You don't need to name the skill - it triggers automatically on any negotiation-shaped request once installed.

## 📦 Install everywhere

The **one-liner above** covers most agents. Here are the manual paths if you want them.

<details>
<summary><b>Claude Code / Claude Cowork</b></summary>

```bash
git clone https://github.com/HemanthGangula/negotiation-coach.git
mkdir -p ~/.claude/skills
cp -r negotiation-coach ~/.claude/skills/negotiation-coach
```
For a project-local install, copy into `.claude/skills/negotiation-coach` inside your repo instead.
</details>

<details>
<summary><b>Claude.ai (web / desktop / mobile)</b></summary>

Settings → Features → Skills → upload a `.skill` file (a zip of this folder). Build one with the packager from [anthropics/skills](https://github.com/anthropics/skills):
```bash
python package_skill.py path/to/negotiation-coach
```
</details>

<details>
<summary><b>Cursor</b></summary>

```bash
git clone https://github.com/HemanthGangula/negotiation-coach.git
mkdir -p .cursor/skills
cp -r negotiation-coach .cursor/skills/negotiation-coach
```
Cursor also auto-discovers skills in `.claude/skills/`, so the Claude Code path works too.
</details>

<details>
<summary><b>Codex CLI · Gemini CLI · Windsurf · Hermes Agent · OpenClaw</b></summary>

Same folder, no changes needed - drop it into the tool's skills directory:
- **Codex CLI:** `~/.codex/skills/negotiation-coach`
- **Gemini CLI:** `npx skills add HemanthGangula/negotiation-coach` (or `~/.gemini/skills/negotiation-coach`)
- **Windsurf / OpenClaw / Hermes Agent:** all read the same `SKILL.md` format - point the tool at this repo or a local clone.
</details>

## 🧠 How it works

The skill doesn't dump a list of tactics - it **sequences** them:

1. **Gets the real situation** - what's being negotiated, where things stand, who's across the table.
2. **Diagnoses BATNA first** - a strong vs. weak alternative changes which tactics are safe to use.
3. **Matches tactics to the phase** - opening, mid-negotiation, or closing - instead of dumping the whole list.
4. **Hands back literal scripts**, not concept names, so there's something you can actually send.
5. **Flags the failure mode** of each tactic so you calibrate instead of overplaying your hand.

See [`SKILL.md`](./SKILL.md) for the full instruction set the agent follows.

## ❓ FAQ

<details>
<summary><b>Is this free?</b></summary>
Yes - MIT licensed. Use it, fork it, modify it, redistribute it.
</details>

<details>
<summary><b>Does it work with my tool?</b></summary>
If your tool reads the <a href="https://agentskills.io"><code>SKILL.md</code></a> format - Claude, Cursor, Codex CLI, Gemini CLI, GitHub Copilot, Windsurf, Cline, Goose, OpenClaw, Hermes Agent, and 30+ others - yes. See <a href="#-install-everywhere">Install everywhere</a>.
</details>

<details>
<summary><b>How is this different from a saved prompt?</b></summary>
An Agent Skill is a version-controlled folder (<code>SKILL.md</code> + reference files) the agent loads <em>only when relevant</em> - not a prompt you paste in every time. It's the same open format Anthropic uses for Claude's built-in skills, released as a standard in December 2025. Only ~50 tokens (name + description) sit in context until the skill actually triggers.
</details>

<details>
<summary><b>Do I need to know negotiation theory?</b></summary>
No. Describe your situation in plain language - the skill does the diagnosis and scripting for you.
</details>

<details>
<summary><b>Is any of this manipulative?</b></summary>
It's built around strategic communication and reading psychology, not deception. It explicitly won't help fabricate facts (like a fake competing offer) - see the ethics note in <a href="./SKILL.md"><code>SKILL.md</code></a>. A good negotiation still ends with both sides able to live with the outcome.
</details>

<details>
<summary><b>Can I use it beyond money?</b></summary>
Some tactics (mirroring, silence, trading-not-giving) generalize to disputes and hard conversations. It's tuned for negotiations with concrete terms, so results are strongest there.
</details>

## 🗂️ Repo structure

```
negotiation-coach/
├── SKILL.md                    # required - frontmatter (name, description) + instructions
├── references/
│   └── tactics.md              # detailed tactic-by-tactic reference, loaded on demand
├── .github/workflows/          # CI: validates SKILL.md frontmatter on every push/PR
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

Follows the [Agent Skills spec](https://agentskills.io/spec): a required `SKILL.md` plus optional `scripts/`, `references/`, and `assets/`. Only the frontmatter (~50 tokens) loads by default; the rest loads only when the skill triggers.

## 🙌 Contributing

New tactics, sharper scripts, new use cases - all welcome. See [CONTRIBUTING.md](./CONTRIBUTING.md).

**If this saved you a few thousand dollars on your next negotiation, [drop a ⭐](https://github.com/HemanthGangula/negotiation-coach) - it's how other people find it.**

## 🔗 Related

- [agentskills.io](https://agentskills.io) - the open Agent Skills specification
- [skills.sh](https://skills.sh) - cross-tool installer (`npx skills add`)
- [anthropics/skills](https://github.com/anthropics/skills) - Anthropic's reference skills & packaging tools
- [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) - community-curated skill directory

## License

MIT - see [LICENSE](./LICENSE). Use it, fork it, remix it.
