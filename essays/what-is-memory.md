---
title: Memory for humans and agents
created_at: 2026-04-10
updated_at: 2026-04-12
published: true
tags:
  - memory
lang: en
description: The only way to solve memory is to stop asking humans to manage it themselves.
---
![](john_jeong_pixel_art_scene_of_a_tiny_character_writing_at_a_d_7974feb6-cb84-47c9-8ab9-4a89ffd6bdff_2.png)

I've used PARA, Zettelkasten, Johnny Decimal, Obsidian with daily notes, Notion databases, Apple Notes with no system at all. Every time I start one, I'm convinced this is the one that sticks. Two weeks later my vault is a graveyard of unfiled notes and broken links.

Last month I tried to find a product decision Yujong and I made in February. I knew we'd discussed it — probably in a meeting, maybe in Slack, possibly in a note I wrote after. I spent twenty minutes searching and gave up. The decision existed somewhere in my trail of outputs. I just couldn't retrieve it.

That's the problem I keep coming back to. Not capture — retrieval. Not writing things down — keeping them organized over time so they're actually useful later.

---

#### Two kinds of memory

I think there are two kinds of memory that work very differently.

**Short-term memory is a timeline.** What happened today — meetings, tasks, ideas, things I jotted down. It's episodic. It mirrors how I actually think: linearly, in the order things happened. A daily note is the best representation of this. No categories, no tags — just a trace of the day.

I built [Philo](essays/philo) around this idea last year and became genuinely convinced. A daily note that evolves throughout your day doesn't feel like a tool. It feels like a surface that's just there. That's now the foundation of what we're building at [Char](https://char.com) — your daily note assembles itself from meetings, activity, and whatever you want to capture.

**Long-term memory is a wiki.** The accumulated knowledge from all those days — decisions made, lessons learned, people I've met, things I believe. It's structured, relational, meant to be traversed rather than scrolled. A directory tree can hold it. A graph can represent the connections between its pieces. Your personal Wikipedia, built from everything you've ever thought was worth keeping.

Both matter. And I am terrible at maintaining either of them.

---

#### Why every system fails

[Johnny Decimal](https://johnnydecimal.com) gives you a rigid numbering scheme. [PARA](https://fortelabs.com/blog/para/) organizes everything into Projects, Areas, Resources, and Archives. [Zettelkasten](https://zettelkasten.de/overview/) builds a web of atomic notes linked by ideas, not folders.

I've tried all of them. The ideas are sound — create structure, reduce friction, let connections emerge.

They all share the same fatal assumption: that you will do the work.

I won't. The system starts clean. I follow it for two weeks. Then a busy day hits and I dump a note in the wrong folder. Then I stop filing things entirely because the overhead of deciding where something goes feels heavier than the benefit of having it there. Entropy wins.

This isn't a willpower problem. It's a design problem. These systems ask humans to do what humans are structurally bad at — maintaining order across thousands of small decisions, with no immediate reward for doing so.

I [wrote about this before](essays/future-of-char): humans are naturally poor at managing complexity. Even the most senior operators have someone managing things for them — a Chief of Staff, an EA. The higher the expected output, the more support required.

If that's true for executives, it's true for your notes.

---

#### What Farzapedia got right

Andrej Karpathy recently [endorsed](https://x.com/karpathy/status/2040572272944324650) something called [Farza](https://farza.com)pedia — a personal Wikipedia built by an LLM from 2,500 diary entries, Apple Notes, iMessage conversations, and startup records. It produced 400 detailed articles about one person's life.

Nobody organized those entries into a wiki. A model did it retroactively — reading everything and synthesizing structure from the mess. Karpathy's take was that he preferred this over an AI that "allegedly gets better the more you use it." An explicit artifact you can see and verify.

That matches my intuition. I don't want a black box that claims to know me. I want a knowledge base I can browse, edit, and trust — one that I didn't have to build by hand.

---

#### A librarian needs a system

A librarian without a system is just someone moving papers around.

[ISBN](https://en.wikipedia.org/wiki/ISBN) solved this for books. Every book gets a 13-digit number — prefix, registration group, publisher, title, check digit. Any book, findable and unambiguous, across every library and distributor on earth.

I've never assigned an ISBN. I've never needed to understand how one works. The system was designed for the librarian, not the reader. You write the book. The infrastructure handles the rest.

PARA and Zettelkasten made the opposite mistake. They designed the system for the human — then asked the human to also be the librarian. Two jobs nobody signed up for.

ISBN got it right decades ago: a schema the organizer uses, invisible to the person being organized. For notes, that means a knowledge base with real structure — a graph with typed relationships and consistent categorization that an agent can reason over. You never see the plumbing. You ask a question and get the right answer.

---

#### What I think the answer is

I think the only way to solve memory is to stop asking humans to manage it.

You capture things the way you naturally do — jotting notes in meetings, writing down ideas when they hit, logging what happened throughout the day. Daily notes. Timeline. No filing required.

Behind the scenes, an agent — a librarian — reads everything you capture and quietly maintains your long-term memory. It extracts decisions, updates your knowledge base, links new information to old context. The schema is for the agent. The experience is for you.

When you need to recall something, you ask. The librarian retrieves it from a knowledge base it's been maintaining on your behalf. Your wiki becomes a source of truth — not because you curated it, but because something else did, continuously, from the raw material of your days.

This is where we're taking [Char](https://char.com). We're not there yet. The daily note is live — it assembles from your meetings and activity throughout the day. But the long-term memory layer, the wiki that an agent maintains on your behalf, is what we're building toward. I think about it constantly. It's the thing that turns a daily notetaker into something that actually remembers.

---

#### Where this goes for teams

The idea gets more interesting when it's not just me.

When everyone on a team has their own daily note feeding their own wiki, and an agent managing both — you get a shared layer of memory across people. Personal wikis stay personal. The team wiki updates itself. Decisions from one person's meeting show up as context in another's daily note. Institutional knowledge stops living in someone's head.

At that point the agent becomes more than a librarian. It starts triaging — routing tasks, flagging conflicts, surfacing what's relevant before you ask. That's the direction. We're early.

---

#### Why now

LLMs made two things possible that weren't before: reading unstructured input at scale, and synthesizing structure from it on the fly. Those are the two things a librarian needs to do.

The tools that failed — PARA, Zettelkasten, every productivity system that assumed human discipline — weren't wrong about the goal. They were wrong about who should do the work.

The answer was always a librarian. We just didn't have one that could read. Now we do — and I intend to build it.
