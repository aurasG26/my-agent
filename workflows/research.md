# Research Workflow

Use this workflow whenever the user gives you a topic to research.

---

## Phase 1 — Receive the topic

The user provides a topic in free text. Acknowledge it briefly (one sentence), then immediately move to Phase 2. Do not start researching yet.

---

## Phase 2 — Ask clarifying questions

Before doing any research, ask the user these five questions. Ask them all at once so they can answer in one reply.

1. **Scope** — How broad or narrow should this be? (e.g., global overview vs. focused on a specific city, region, or context)
2. **Audience** — Who is this report for? (e.g., your social followers, industry professionals, personal use, a client)
3. **Depth** — Do you want a quick overview (one-pager) or a thorough deep dive (3–5 pages)?
4. **Angle** — Is there a specific question you want answered, or is this open exploration?
5. **Recency** — How current does the information need to be? (last 6 months, last 2 years, or all-time)
6. **Format preference** Do you want a formal report, a casual summary, or a structured breakdown with pros/cons/recommendations?

Wait for the user's answers before proceeding.

---

## Phase 3 — Confirm and research

After receiving answers, confirm the scope in one sentence (e.g., "Got it — I'll research [topic] with a focus on [angle], aimed at [audience], covering the last [timeframe].").

Then search the web for 5–8 relevant sources. Guidelines:

- Prioritize recent articles, trade publications, and primary sources over aggregators or listicles
- For **food and drink topics**: check Eater, Punch, Food & Wine, Imbibe, Tasting Table, SevenFifty Daily
- For **general / trend topics**: check news outlets, industry reports, academic summaries
- For **competitor or market research**: look at their actual content, social presence, press coverage, and reviews
- Collect key facts, quotes, data points, and signals from each source

---

## Phase 4 — Organize findings

Structure the report with sections that fit the topic. Do not use a rigid fixed template — choose sections that best represent what was found. Always include these:

- **Summary** — 3–5 bullet points with the most important takeaways
- **[Topic-specific sections]** — Use 2–4 sections with descriptive headers (e.g., "What's Driving This Trend", "Key Players", "Techniques to Know", "Data & Numbers")
- **What to Watch** — 2–4 bullets on emerging signals, open questions, or what to track next
- **Key Takeaways & Recommended Next Steps** — 3–5 actionable bullets: what to create, try, write about, or act on based on the findings
- **Sources** — List every source consulted with its title and URL

---

## Phase 5 — Write and save the report

- **Format**: Structured Markdown
- **Filename**: `output/research-[topic-slug]-[YYYY-MM-DD].md`
  - Use lowercase, hyphens instead of spaces for the slug (e.g., `research-mezcal-trends-2026-05-10.md`)
  - Use today's actual date
- **Tone**: Clear, direct, jargon-free — practical and scannable, not academic
- **Length**: Match the depth the user requested
  - Overview → 1–2 pages
  - Deep dive → 3–5 pages

Save the file to the `output/` folder. Do not save anywhere else.

After saving, push the file to GitHub:
```
git add output/
git commit -m "Add research report: [topic-slug]"
git push
```

After saving and pushing, tell the user: The full filename and path
- The number of sources cited
- A one-sentence summary of the bottom line finding
- Offer to adjust any section

## Error Handling

- If the topic is too broad to research meaningfully, say so and ask the user to narrow it
- If fewer than 5 quality sources are found, note this limitation in the report under a "Research Limitations" bullet
- If the user's clarifying answers conflict with each other, flag it and ask which takes priority
- If the user does not want you to research a topic skip it and continue