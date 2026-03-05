# Inbox-to-Execution Pipeline

**What it does:** Processes your inbox, drafts responses in your voice, tags and categorizes emails, and flags anything that needs your decision.

**Connectors needed:** Gmail or Email

**Best as:** Daily recurring task (schedule for 30 min before you start work)

---

## One-Time Setup Prompt

```
I want to set up a daily inbox processing workflow.

Every morning, you should:
1. Read all new/unread emails from the last 24 hours
2. Categorize each email by type: Client, Internal, Sales, Admin, Urgent
3. For important emails, draft a response matching my tone from brand-voice.md
4. Flag anything that needs my decision before responding
5. Create a daily briefing summary

Output format:

🔴 URGENT — Action Required
[List emails that need immediate attention with recommended action]

📧 DRAFTED RESPONSES — Ready for Review
[Email summary → drafted response for each]

🏷️ TAGGED & SORTED
[Table: Sender | Subject | Category | Priority (High/Medium/Low)]

📋 DAILY SUMMARY
- X emails processed
- X responses drafted
- X flagged for my decision
- X low-priority (archived/skipped)

Save the briefing to /outputs/daily-inbox/YYYY-MM-DD-inbox-briefing.md

Before starting, confirm you can access my email and show me your plan.
```

---

## To Make It Recurring

```
/schedule

Run my inbox processing workflow every weekday at 7:30 AM.
Follow the same process and output format each time.
Save each briefing to /outputs/daily-inbox/ with the date in the filename.
```

---

## Tips

- **Refine the categories** to match your actual email types after the first run
- **Add specific rules** like: "Emails from [client domain] are always High priority"
- **Update brand-voice.md** if the drafted responses don't sound like you — that's a context problem, not a prompt problem
