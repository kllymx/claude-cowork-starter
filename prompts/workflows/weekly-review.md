# Weekly Operating Review Builder

**What it does:** Pulls data from your project management tools, communication channels, and notes to generate a structured weekly review — wins, blockers, risks, and recommended decisions.

**Connectors needed:** Notion, Slack, and/or ClickUp/Smartsheet/Airtable (use whichever you have)

**Best as:** Weekly recurring task (schedule for Monday AM or Friday PM)

---

## The Prompt

```
Build my weekly operating review for the past 7 days.

Pull from:
- Slack: key updates, decisions, and open questions from my main channels
- Notion: project status, task completions, and any updated pages
- Calendar: meetings held this week and any upcoming deadlines

Structure the review as:

## Weekly Operating Review — [Week of DATE]

### ✅ Wins
[What shipped, what progressed, what closed]

### 🚧 Blockers
[What's stuck, who's waiting on what, what's overdue]

### ⚠️ Risks
[What could go wrong this week, what needs attention before it becomes a problem]

### 🔗 Dependencies
[What's waiting on someone else, cross-team handoffs, external blockers]

### 💡 Recommended Decisions
[Based on what you've seen, what should I prioritize, deprioritize, or escalate?]

### 📅 Next Week Preview
[Key meetings, deadlines, and deliverables coming up]

If any data source is unavailable, note what's missing rather than guessing. Mark anything you're less than 80% confident about as VERIFY.

Save to /outputs/weekly-reviews/YYYY-MM-DD-weekly-review.md
```

---

## To Make It Recurring

```
/schedule

Run my weekly operating review every Monday at 8:00 AM.
Follow the same structure each week.
Save to /outputs/weekly-reviews/ with the date in the filename.
```

---

## Tips

- **The first run won't be perfect.** Use it to calibrate — tell Claude what it got wrong and update your context files accordingly.
- **Add a Folder Instruction** in your weekly-reviews folder: "Review previous weeks' reports in this folder for context on ongoing themes and recurring blockers."
- **Use subagents for speed:** Add "Spin up subagents to pull from each data source in parallel" if you have 3+ connectors.
