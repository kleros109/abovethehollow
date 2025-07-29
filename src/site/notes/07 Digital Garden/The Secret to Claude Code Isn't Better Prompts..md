---
{"dg-publish":true,"permalink":"/07-digital-garden/the-secret-to-claude-code-isn-t-better-prompts/","tags":["readwise"],"updated":"2025-07-28T19:22:59.002-07:00"}
---

# The Secret to Claude Code Isn't Better Prompts...

![rw-book-cover](https://pbs.twimg.com/profile_images/1912749702828945408/kgtfnQn4.jpg)

- URL: https://twitter.com/tomcrawshaw01/status/1948744096404644067/?rw_tt_thread=True
## Summary
The secret to Claude Code is not just better prompts. It helps Claude understand your codebase first. This system took eight months to build.

## Highlights
### id918933637

> ![](https://pbs.twimg.com/media/GwtUXj3bkAASdaH.jpg)

 * [View Highlight](https://read.readwise.io/read/01k13zm097xar26d24qpkdzqm6)

# After 8 months of daily AI coding, I built a system that makes claude code actually understand what you want to build


I’ve been pair programming with AI coding tools daily for 8 months writing literally over 100k lines of in production code. The biggest time-waster? When claude code thinks it knows enough to begin. So I built a requirements gathering system (completely free and fully open sourced) that forces claude to actually understand what you want utilizing claude /slash commands.

## The Problem Everyone Has:

• You: “Add user avatars”
• AI: *builds entire authentication system from scratch*
• You: “No, we already have auth, just add avatars to existing users”
• AI: *rewrites your database schema*
• You: *screams internally and breaks things*

## What I Built:

A /slash command requirements system where Claude code treats you as the product manager that you are. No more essays. No more mind-reading.

## How It Actually Works:

1. You: `/requirements-start {Argument like "add user avatar upload}`
2. AI analyzes your codebase structure systematically (tech stack, patterns, architecture)
3. AI asks the top 5 most pressing discovery questions like “Will users interact through a visual interface? (Default: YES)”
4. AI autonomously searches and reads relevant files based on your answers
5. AI documents what it found: exact files, patterns, similar features
6. AI asks the top 5 most clarifying questions like “Should avatars appear in search results? (Default: YES - consistent with profile photos)”
7. You get a requirements doc with specific file paths and implementation patterns

## The Special Sauce:

• **Smart defaults on every question** - just say “idk” and it picks the sensible option
• **AI reads your code before asking** - lets be real, claude.md can only do so much
• **Product managers can answer** - Unless you’re deep down in the weeds of your code, claude code will intelligently use what already exists instead of trying to invent new ways of doing it.
• **Links directly to implementation** - requirements reference exact files so another ai can pick up where you left off with a simple /req… selection

## Controversial take:

Coding has become a steering game. Not a babysitting one. Create the right systems and let claude code do the heavy lifting.

Full repo with commands and examples and how to install (no gate but would appreciate a start if it helped you):
<github.com/rizethereum/claude-code-requirements-builder>

**Special shout out:** This works best with <https://repoprompt.com/> codemaps, search, and batch read mcp tools but can work with out them.​​​​​​​​​​​​​​​​