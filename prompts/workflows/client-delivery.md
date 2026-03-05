# Client Delivery Pack Generator

**What it does:** Takes your raw project materials — notes, docs, prior updates — and produces a polished client status report, next-phase plan, and follow-up email draft.

**Connectors needed:** Google Drive or Notion (optional — works with local files too)

**Best as:** On-demand or weekly recurring task per client

---

## The Prompt

```
Create a client delivery pack using the materials in /projects/[client-name]/.

Read all files in the folder. Check _MANIFEST.md if it exists for priority ordering.

Produce:

## 1. Status Report
- Executive summary (3-4 sentences max)
- Work completed this period
- Key milestones hit or missed
- Metrics or results (if available in the source materials)

## 2. Next Phase Plan
- What's coming next
- Key deliverables and estimated timelines
- Dependencies or decisions needed from the client
- Any risks or assumptions

## 3. Open Questions
- Unresolved items that need client input
- Decisions we're waiting on
- Anything ambiguous in the project materials (flag as VERIFY)

## 4. Follow-Up Email Draft
- Draft a concise email to the client summarizing the update
- Match my tone from brand-voice.md
- Include the status report as an attachment reference
- End with a clear next step or call to action

Save all outputs to /outputs/client-deliverables/[client-name]/YYYY-MM-DD/

If anything in the source materials is unclear or contradictory, flag it — don't resolve it by guessing.

Show me your plan before executing.
```

---

## Tips

- **Create a _MANIFEST.md** in each client folder so Claude reads the current brief and latest updates first, not old drafts
- **Add client-specific Folder Instructions:** "Client uses 'platform' not 'app'. Tone: professional but warm. Key contact: [name], [role]."
- **Iterate the email draft** — if the tone is off, update brand-voice.md with a client communication example
