---
title: Your meeting notes are a dead end
created_at: 2026-04-09
updated_at: 2026-04-13
published: true
tags:
  - startup
lang: en
description: Transcripts don't carry anything forward. We're building the thing that does.
---
I wrote about [where Char is heading](future-of-char) and then about [the mistakes we made getting here](lessons-from-shipping). This one is about the product itself.

*This is where we're headed, not where we are today. Char is still in active development.*

---

#### The problem nobody has a good tool for

Meeting notetakers are a solved category. Granola just [raised at $1.5B](https://www.granola.ai/blog/series-c). Otter, Fireflies, Fathom — they all do transcripts and summaries. The feature set is converging. Competing on transcript accuracy is a race to parity.

But every day I hit the same thing: the meeting ends and everything scatters. Three action items got spoken out loud. A design decision got made. Someone said "let's circle back on pricing." Then I open Slack, open Linear, open my notes app, and try to manually reconstruct what matters. Half of it lives in my head. Some of it I forget entirely.

I have a task manager, a notetaker, and a CRM. They don't talk to each other. My task manager doesn't know what was said in the meeting and my meeting notes don't reference last week's decisions. Every tool has a piece. No tool has context across all of them.

The more meetings I take, the worse this gets. I spend hours every day just triaging — organizing, remembering, routing. Not the work itself, the meta-work around it. Even the most senior operators I know have someone managing this for them — a Chief of Staff, an EA. The rest of us just deal with it.

The real question was never how to capture a meeting. It's who carries forward everything a meeting produces.

---

#### What Char actually is

Char starts with meetings and ends with everything that flows from them. The core is the **daily note**.

This didn't arrive fully formed. Yujong and I spent three weeks of working sessions building conviction around it. On March 21st we first discussed the daily note as the home screen — a "compass" for your day, with calendar events appearing as chips linked to real meetings. Two days later we dug into task ingestion — how items from Linear and GitHub could auto-surface, how email triage would work, how slash commands could let you pull in context.

By March 31st we'd aligned on making it the actual home screen, with the existing sidebar declared redundant and the recording button embedded directly in the daily note. April 2nd it crystallized: the daily note is the foundation for an autonomous "COO"-level assistant. At our all-hands four days later, the line that stuck: "Meeting notes is going to be a feature of Char, whereas before it was the product itself."

I built [Philo](philo) last year and became bullish on this idea. A daily note that evolves throughout your day doesn't feel like a tool. It feels like a surface that's just always there.

In Char, the daily note assembles itself. You finish a call and action items land in your daily note, not in a separate meetings tab. You work on your computer and Char logs what happened to your timeline, like [Openbird](openbird) but woven into the note itself. Quick thoughts go in the same place. Everything from that day, in one surface.

Over time it becomes your working memory — what you did, what you decided, what's still pending.

---

#### Why this isn't another notetaker

A meeting notetaker gives you a record of what was said. Char gives you a system that remembers what was *decided*, connects it to what came before, and helps you act on it.

Meeting notetakers optimize for capture — transcript accuracy, speaker detection, summary quality. We optimize for **continuity** — context carrying forward across days, across meetings, across people. That's a different product with a different architecture.

On March 27th, Yujong and I looked at the competitive landscape — [Pocket](https://www.ycombinator.com/companies/pocket), [Caretta](https://www.ycombinator.com/companies/caretta), [Button](https://www.ycombinator.com/companies/button-computer), all arriving in one YC batch with transcription baked in but none of them selling it as the product — and agreed that transcription-only positioning is commoditized. On April 3rd we discussed how live transcripts have less value than live summaries, and that users we'd interviewed were fine with results arriving after the meeting. The transcript matters. But it's the input, not the output.

A power user in our Discord made the best case against this:

> *"I already have an executive assistant skill that gives me daily briefs via Claude Code. It reads through my emails, Slack messages, Jira, and Hyprnote (our former name) transcripts and generates a task list. I can easily swap out any single tool in the chain."*

Fair. You can DIY this. But every tool in that chain is stateless. Claude Code doesn't remember yesterday's brief and Jira doesn't know what was said in the meeting. The chain works once — it doesn't compound.

Char's value isn't the daily note as a format. Anyone can write a daily note in Obsidian. The value is the context layer underneath. Tuesday's note has context from Monday's. Thursday's meeting note references a decision from Tuesday's. When you ask "what did we decide about pricing?" Char doesn't search a folder of markdown files — it traverses a graph of context that's been building for weeks.

That's the piece you can't replicate by chaining disconnected tools.

---

#### What it looks like — and what it actually is

From the outside, Char is a timeline-based notetaking app. You open it, you see a page. You type, you take meetings, you jot things down. Integrations and automations are batteries included — not plugins you configure, just things that happen.

Char looks like a notepad. It's actually an agent that reads your mind.

Underneath, a system reads your context across every stream it touches — meetings, screen activity, tasks, emails, calendar — and infers what matters. The daily note is a trojan horse for context capture. People want to write on it, and the writing is the data.

It's also bundled with a CLI, which makes it just as native for AI agents as it is for humans. A person opens the GUI and types. An agent calls the CLI and reads. Same data, two interfaces.

---

#### How it compounds

One person starts using Char. Daily notes, meetings, quick thoughts. The AI connects what you said at 10am to what someone emailed at 3pm, surfaces the follow-up you forgot about. You start relying on it.

Then you bring in your team. Everyone gets their own daily note. The AI now sees across all of them — triaging, routing decisions, flagging what's blocked. It stops being a personal tool and becomes shared infrastructure.

That's where it gets hard to leave. A solo daily note is replaceable — anyone can build one. But once the AI is managing context between people, removing it means losing months of accumulated organizational memory. That's not a feature. That's a foundation.

---

#### How we're going to market this

The product is harder to explain than "AI meeting notetaker". That was a clean pitch. "Command center powered by daily notes" is not.

**Lead with meetings, not the daily note.** Meetings are where people feel the pain. That's what they're searching for. The pitch at the top of the funnel: *Char captures your meetings and turns them into action — not just notes.* Concrete enough to be interesting, familiar enough not to confuse.

Once someone uses Char for their first meeting and sees action items show up in their daily note, the product sells the next step on its own. They don't need to understand the full vision on day one.

**The activation moment is day two.** The first meeting is adoption. The second morning is retention. If someone opens Char the morning after their first recorded meeting and finds a daily note with yesterday's action items already there — context from the meeting, a sense that this thing remembers — that's the click.

Most notetakers are session-based. You record, you get a summary, you leave. Char's bet is on *returning*. The daily note only works with continuity. Day one is useful. By the end of the first week, it's hard to leave.

**The persona is the back-to-back founder — but I'll be honest, we're still narrowing this.** At our April 6th all-hands, Artem pushed back that "founders" is too broad as a target. He's right. Yujong reframed it: instead of locking in a single persona, define what Char will *not* do and who it will *not* serve. I don't have a clean answer yet.

What I do know: the ideal user has 4+ meetings a day, no EA, and has given up on staying on top of things. Their calendar is a wall of color. They've tried task managers and notetakers and the actual problem — that everything is disconnected — was never solved. Whether that's a seed-stage founder, a senior PM, or a managing director at a consulting firm — I'm not sure yet. We'll learn by shipping and watching who retains.

**Content is the channel.** I'm writing these essays because I think the most effective marketing for Char right now is showing our thinking publicly. Founders follow founders who think clearly about problems they share. If I can describe the problem well enough that people see themselves in it, the product pitch becomes obvious.

We'll ship a public changelog, share process on Twitter, do short demo videos of the daily note in action. But the foundation is writing — because writing forces clarity, and clarity is what sells a product you can't screenshot.

---

#### What's next

Cloud sync ships this month. SQLite migration and folders after that. These have been the blockers since March — Yujong and I have flagged SQLite as the single largest dependency in nearly every working session. Sync depends on it. Folders depend on it. The daily note depends on it. I'm not going to pretend this is a clean Phase 1 → Phase 2 → Phase 3 sequence. The reality is Phase 1 has been stuck, and we're now unsticking it.

After that: the daily note as the entire product, not a feature inside the product. If people don't open Char in the morning because the daily note is the best way to start their day, nothing else we build matters.

After that: agentic handoffs. You finish a meeting, action items surface, and Char routes them — spec to Cursor, design decision to your co-founder's daily note, follow-up email drafted for review. By the time you're in the next meeting, the work is already moving.

There's also something we haven't talked about publicly yet: we've been exploring a hardware dongle for always-on meeting detection. The current system only responds to scheduled remote meetings, which means spontaneous in-person conversations — often the most important ones — get missed entirely. Yujong and I have spent multiple sessions on this: VAD-based activation, a two-tier mic strategy where the dongle acts as a sentinel and triggers the MacBook's higher-quality mic when speech is detected, minimal firmware, ~$20 BOM at 100 units. It's early — April for research, May for a first version. But if it works, it fills a real gap in the daily note's coverage.

The wedge is the daily note. Everything else is downstream. The endgame isn't a notetaking app — it's the memory layer for you, your team, and every agent working on your behalf.
