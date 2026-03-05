# Sales Follow-Up and Objection System

**What it does:** Takes discovery notes, CRM context, and past outreach to generate tailored follow-up messages, objection responses, and next-step sequences.

**Connectors needed:** HubSpot or CRM (optional — works with pasted notes too)

**Best as:** On-demand after calls, or batch process weekly

---

## Single Follow-Up Prompt

```
I just had a discovery call. Here are my notes:

[Paste your call notes, or point to a file: "Read /projects/sales/[prospect-name]-notes.md"]

Based on these notes, create:

## 1. Follow-Up Email
- Reference specific points from our conversation (not generic)
- Match my tone from brand-voice.md
- Include a clear, specific next step
- Keep it under 150 words

## 2. Objection Responses
- Identify the top 2-3 likely objections based on what was discussed
- Draft a response for each that's direct, not defensive
- Include proof points or examples where relevant

## 3. Next-Step Sequence
- If they respond positively: what's the next email/action?
- If no response in 3 days: draft a follow-up nudge
- If they push back: draft a re-engagement approach

Save to /outputs/sales/[prospect-name]/YYYY-MM-DD-followup.md

If anything from the call notes is ambiguous, flag it as VERIFY rather than assuming.
```

---

## Batch Processing Prompt

```
Process all files in /projects/sales/pending-followups/.

For each prospect file:
1. Read the notes
2. Generate a tailored follow-up email
3. Identify top objections and draft responses
4. Recommend a next step

Spin up subagents to process each prospect in parallel.

Save individual outputs to /outputs/sales/[prospect-name]/ and create a summary table:

| Prospect | Company | Stage | Recommended Action | Follow-Up Ready? |
|---|---|---|---|---|

Save the summary to /outputs/sales/YYYY-MM-DD-pipeline-actions.md
```

---

## Tips

- **Install the Sales plugin** alongside this workflow for access to `/sales:call-prep` and `/sales:battlecard` commands
- **Stack with Data Analysis plugin** to analyze pipeline patterns: "Which deal stages have the highest drop-off?"
- **Build a prospects template** in your projects folder so discovery notes are consistently structured — Claude produces better output from consistent inputs
