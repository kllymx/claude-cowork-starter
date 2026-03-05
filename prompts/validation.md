# Validation Prompt

**Run this after setting up your context files and global instructions. It confirms Claude has loaded everything correctly before you start real work.**

If the summary comes back wrong, fix your context files first. Bad setup compounds quickly.

---

## The Prompt

```
Read all files in /context and review my global instructions.

Summarize:
1. What you know about me (role, priorities, domain)
2. How I prefer to work (process, output style, communication)
3. What guardrails you should follow (safety rules, non-negotiables)
4. What my communication style sounds like (tone, words I use, words I avoid)

Do not begin any other work yet.

If anything seems incomplete or contradictory, flag it so I can fix it now.
```

---

## When to Re-Run This

- After any major update to your context files
- When starting a new project folder with folder-specific instructions
- If Claude's output suddenly feels off — usually means context drifted
