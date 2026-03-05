# Content Repurposing Operator

**What it does:** Takes one piece of long-form content (article, video transcript, podcast notes, presentation) and generates multiple platform-specific outputs — LinkedIn posts, email newsletters, short-form hooks, and more.

**Connectors needed:** None required (works with local files)

**Best as:** On-demand after publishing any long-form content

---

## The Prompt

```
Repurpose the following content for multiple platforms:

[Paste your content, or point to a file: "Read /projects/content/[filename].md"]

Using my brand voice from brand-voice.md, create:

## 1. LinkedIn Post Variants (3 options)
- Variant A: Hook-driven (open with a bold or provocative statement)
- Variant B: Story-driven (open with a specific example or anecdote from the content)
- Variant C: List-driven (key takeaways as a scannable list)
- Each should be 150-250 words
- End each with a question or CTA that drives comments

## 2. Email Newsletter Draft
- Subject line (3 options)
- Preview text
- Body: conversational summary of key points, linking back to the full piece
- CTA at the end
- 300-500 words max

## 3. Short-Form Hooks (5 options)
- One-liner hooks suitable for X/Twitter, Instagram captions, or thread openers
- Each should be punchy, standalone, and make someone want to read more
- Under 280 characters each

## 4. Key Quotes
- Pull 3-5 quotable lines directly from the original content
- These should work as standalone graphics or pull quotes

Save all outputs to /outputs/content/[content-title]/YYYY-MM-DD-repurposed.md

Match my voice exactly. If the tone drifts from brand-voice.md, flag it.
```

---

## Tips

- **Run this every time you publish anything.** One article should generate a week of content across platforms.
- **Add platform-specific notes** to brand-voice.md: "LinkedIn: more professional, longer form. X: punchier, more direct. Email: conversational, like writing to a smart friend."
- **Stack with the Marketing plugin** for access to `/marketing:draft-content` and platform-specific optimization
- **Feed the best-performing variants back into brand-voice.md** — if Variant A consistently gets more engagement, that tells you something about your audience
