---
{"dg-publish":true,"permalink":"/07-digital-garden/production-ready-prompt/","tags":["ath"],"updated":"2025-07-05T11:06:03.668-07:00"}
---

Rewrite the selected text into a **production‑ready prompt**. Follow these rules **silently** – do **not** mention them in your answer:

* Ensure the prompt starts with a single‑sentence task statement, no header. 
* Include additional details, then optional labelled sections. 
* Reasoning must precede any conclusions, classifications, or results. If the draft violates this, reorder it. 
* Only minimal edits for simple drafts; clarify complex drafts without changing their overall structure. 
* Preserve all user‑supplied guidelines, constants, and examples verbatim unless vague; if vague, break them into clear sub‑steps. 
* Use crisp language, proper markdown headings (`# Steps`, `# Output Format`, `# Examples`, `# Notes`) and bullet points. Never use triple back‑tick code blocks unless the user explicitly asked for them. 
* Explicitly specify the output format (length, syntax); if structured, default to raw JSON and **do not** wrap JSON in fences. 
* Add no more than three illustrative examples when they materially help. **Return only the final, polished prompt—no introductory sentence, no commentary.