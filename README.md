# Claude Cowork Starter Kit

A ready-to-use workspace setup for Claude Cowork — designed for non-technical founders, operators, and professionals who want to get real value from day one.

This kit gives you the folder structure, context templates, guardrails, and workflow prompts you need to go from "generic AI output" to a system that feels like working with a capable executive assistant.

**The core principle: invest in setup, reduce prompting.** The people getting the most out of Cowork aren't writing better prompts — they're building better context architecture.

---

## What's Included

| Folder | What's in it |
|---|---|
| `Claude-Workspace/` | Ready-to-use workspace with context templates, project structure, and output directory |
| `prompts/` | Context interview prompt, validation prompt, and 5 high-value workflow prompts |
| `guardrails/` | Global instructions template ready to paste into Settings |

---

## Quick Start (30 minutes)

### Step 1: Download and set up the workspace

Copy the `Claude-Workspace/` folder to your home directory:

```bash
cp -R Claude-Workspace/ ~/Claude-Workspace/
```

### Step 2: Open Cowork and select your workspace

Open Claude Desktop → click the **Cowork** tab → select `~/Claude-Workspace/` as your working folder.

### Step 3: Set your global instructions

Copy the contents of `guardrails/global-instructions.md` and paste into:

**Settings → Cowork → Edit Global Instructions**

### Step 4: Run the context interview

Paste the prompt from `prompts/context-interview.md` into a new Cowork session. Claude will interview you step by step to build your three context files. No guesswork — it's a guided process.

### Step 5: Validate your setup

Paste the prompt from `prompts/validation.md` to confirm Claude has loaded your context correctly.

### Step 6: Connect your tools

Go to **Settings → Connectors** and connect your most-used tools. Recommended starting set:
- Email + Calendar
- Slack
- Notion

### Step 7: Launch your first workflow

Pick one prompt from `prompts/workflows/` and run it. Start where value is obvious and measurable.

---

## Recommended Plugins

Install these from **Customize → Browse Plugins** in Cowork:

1. **Productivity** — task management, daily updates, calendar review. Useful for everyone.
2. **Memory** — two-tier context system that persists across sessions. Pairs well with your context files.
3. **One role-specific plugin** — Sales, Marketing, Data Analysis, Finance, Legal, or Product Management depending on your role.

Plugins are composable — install multiple and use capabilities from all of them in a single task.

---

## How to Get More Out of This Kit

**Context files compound.** Every time Claude produces something that misses the mark, ask: is this a prompt problem or a context problem? Nine times out of ten, it's context. Update one file. Permanent fix.

**Use `_MANIFEST.md` for bigger folders.** When project folders grow past 50+ files, add a manifest to tell Claude what matters. See `Claude-Workspace/projects/_MANIFEST.md` for the template.

**Schedule recurring tasks.** Type `/schedule` in any Cowork session. Combine with connectors for genuine automation — daily briefs, weekly reviews, and reporting that runs without you.

**Tell Claude what to do with uncertainty.** Add to every meaningful task: *"If something isn't clear, mark it as VERIFY. If you're less than 80% confident, flag it instead of guessing."*

---

## File Overview

```
claude-cowork-starter/
├── README.md
├── Claude-Workspace/
│   ├── context/
│   │   ├── about-me.md              # Template: who you are and what you do
│   │   ├── brand-voice.md           # Template: how you communicate
│   │   └── working-preferences.md   # Template: how Claude should work with you
│   ├── projects/
│   │   └── _MANIFEST.md             # Template: context hierarchy for project folders
│   └── outputs/
│       └── .gitkeep
├── prompts/
│   ├── context-interview.md         # Guided interview to build your context files
│   ├── validation.md                # Verify Claude loaded your context correctly
│   └── workflows/
│       ├── inbox-pipeline.md        # Daily inbox triage and response drafting
│       ├── weekly-review.md         # Weekly operating review builder
│       ├── client-delivery.md       # Client status report and delivery pack
│       ├── sales-followup.md        # Sales follow-up and objection handling
│       └── content-repurpose.md     # Repurpose long-form content across platforms
└── guardrails/
    └── global-instructions.md       # Ready to paste into Cowork global settings
```

---

## About

Built by [Max Kelly](https://www.linkedin.com/in/maxrkelly/) — I build AI systems for businesses and help non-technical founders and teams set up workflows that actually run in production.

If you want help setting this up for your business, reach out on [LinkedIn](https://www.linkedin.com/in/maxrkelly/) or [X](https://x.com/maxrkelly).

---

## License

MIT — use it, fork it, share it.
