# Self Manual · 自我说明书

**Version 1.0.0** · [Changelog](CHANGELOG.md)

**Not a test of who you are. A companion that helps you remember yourself, one moment at a time.**

Self Manual is a bilingual (English / 中文) skill for Claude. Instead of handing you a personality type, it interviews you about things that actually happened (the evening that felt unexpectedly good, the meal you still think about, the party that drained you) and slowly writes a **personal user manual** with you: what makes you happy, where you feel at ease, what drains your battery, how you like to rest, what you're good at, what you need from people, and what you're still figuring out.

[中文说明 →](README.zh.md)

## Why it's different

- **Real moments, not self-ratings.** People are bad at summarizing themselves but good at remembering specific days. Every entry comes from something you lived.
- **Nothing is written without your OK.** The AI's interpretations are labeled as guesses. You confirm, edit, or delete every line.
- **Evidence, not labels.** Entries keep the facts behind them, counterexamples, and a confidence level (✅ confirmed, 🔸 guess, ❓ still exploring), so your manual can change as you do.
- **It knows when to stop.** "I love hotpot" gets noted, not interrogated. Deeper questions only come when there's something worth unpacking and you're up for it.
- **Playful, not preachy.** Rapid-fire this-or-that, fill in the blanks, a mystery-box question, "your user manual: gadget edition". It gets quieter when you're having a hard day.
- **Honest about messy feelings.** Jealousy, vanity, and contradictions get explored with curiosity, not polished into fake positives.

## What you can do with it

| Mode | What happens |
|------|--------------|
| Easy warm-up | Five small memories, about 10 minutes, and you get a first draft |
| Deep dive | Pick one of nine areas: happy moments, comfortable spaces, food, energy, rest and taste, strengths, relationships, values, stuck points |
| Import | Paste an old AI chat or your notes and get an initial manual (old AI conclusions start as guesses) |
| Daily question | One light question a day, two minutes |
| Preference lab | Turn a guess into a tiny real-life experiment, then update the manual |
| Blind spots | Once you have enough entries, gently tests conclusions that seem to contradict each other |
| Life guide | Turns your manual into practical notes: your ideal week, what helps you recover, what to weigh in big decisions |

## Install

1. Download `self-manual.skill` (or the `self-manual` folder) from this repo.
2. **Claude app (web / desktop):** upload the file in Settings, under Skills.
   **Claude Code:** put the `self-manual` folder in `~/.claude/skills/`.
3. Start a new chat and say something like *"I want to write a user manual about myself"* or *"help me figure out what I actually like."*

It works in English or Chinese. Claude replies in whatever language you write in.

## Keep your manual

A skill doesn't remember anything between chats on its own. At the end of each session, Claude gives you the updated manual. Save it in a notes app or a doc, then paste it back next time to keep going.

## A taste

> **Claude:** In the last three months, was there an evening you got home and thought, "Today was actually pretty good"?
> **You:** Maybe the Saturday I spent at a café. I didn't even do much.
> **Claude:** Was it the café itself, or the fact that nobody needed anything from you that day?
> **You:** …the second one, honestly.
> **Claude:** Dropping this in the pocket as a guess, not a fact yet: 🔸 *you recharge best around people who don't need anything from you.* Sound right, or should I change the wording?

## Boundaries

This is a self-reflection tool, not therapy or diagnosis. It doesn't infer health or mental-health conditions. Your manual belongs to you: delete anything, any time. If a conversation touches real distress, it pauses the process and suggests reaching out to people you trust or a professional.

## Files

- `SKILL.md`: entry point, modes, language routing
- `persona.md` / `en/voice.md`: voice and example lines (Chinese / English)
- `start.md`, `interviewer.md`, `inference-rules.md`, `feedback.md`, `lab.md`, `life-guide.md`, `manual-template.md`: how it interviews, concludes, wraps up, experiments
- `questions/zh/`, `questions/en/`: question banks for nine areas plus games, each with ☀️ easy / 🌤️ deeper / 🌙 late-night levels
