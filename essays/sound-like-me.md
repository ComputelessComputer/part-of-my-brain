---
title: Sound like yourself
created_at: 2026-04-17
updated_at: 2026-04-17
published: true
tags:
  - writing
  - ai
lang: en
description: I spent a weekend trying to make my writing sound less like AI. I had the objective wrong.
---
I spent a weekend trying to make my writing sound less like AI. Every revision came out more uncanny than the last.

Then I realized I had the objective wrong.

---

**The wrong target**

"Doesn't sound like AI" is a negative space. Infinite. You optimize against whatever the current detector or reader happens to flag this month, and the output lands as generic-human-voice slop. Still eerie, just differently eerie.

"Sounds like me" is a target. Specific. Grounded. You can measure against it.

I didn't understand this until I built a skill that got it wrong.

---

**The skill that almost worked**

I had two Claude Code skills I liked — a humanizer and a stop-flop scorer. Both solid on their own. I merged them into one slash command so I wouldn't have to run them twice. I called it [audit](https://github.com/ComputelessComputer/audit).

The foundation was good. Pattern libraries, scoring categories, the usual tells from the Wikipedia post on AI-generated writing. I ran it on my own drafts.

The output was polished. It read like a competent stranger wearing my clothes.

That was the moment it clicked. The skill had no idea what "me" was. It was sanding off AI-ness into a generic human voice — and generic human voice, it turns out, still smells like AI. The absence of authorial specificity is what actually flags something as machine-made. Not word choice. Not em-dashes. Specificity.

---

**Grounding fixed it**

I pointed Claude Code at everything I'd written before GPT-3.5 came out. Old essays. Raw journal dumps. Drafts I never published.

I'm glad I didn't trust my own intuition about my voice, because the model found patterns I wouldn't have articulated. A bias toward shorter sentences when the point is sharp. A habit of admitting the failure before stating the lesson. Alternation between punch and explain. These are things I do. I just couldn't have told you I did them.

AI is extraordinary at pattern extraction. Humans are bad at articulating their own voice. That inversion is the whole game.

I had the model quote real snippets from my writing, turn them into a `references/` folder, and wrote an instruction file describing the structure and tone — grounded in concrete examples, not adjectives. Then I reran audit.

The next draft sounded exactly like me. Just sharper.

---

**The hybrid is already here**

Here's the part people don't want to say out loud.

Every piece of writing that ships from now on is going to be some mixture of AI-written and human-written. Not because AI is winning. Because the line was never clean. Every writer has always used tools — spellcheck, editors, their own internal editor on the third pass. The model is the newest one.

So the interesting question isn't whether AI touched the draft. It's whether the draft still sounds like the person whose name is on it.

The way you keep sounding like yourself at scale is by giving the model a real reference of who you are. Not a style guide. Not vibes. Your actual writing, quoted back at you.

---

**Personal instructions are the moat**

If everyone prompts the same foundation model with the same generic "make this sound human" instruction, everyone gets the same voice. That voice is the one getting flagged as AI — not because it's AI, but because it's nobody in particular.

Ground the model in your own prior work and the output stops being a generic human. It starts being you. More polished than you'd write alone. Still yours. That's not cheating. That's what tools are for.

The writers who stand out in the next few years won't be the ones who avoided AI. They'll be the ones who built good personal instructions — and kept writing enough raw material to feed them.

---

Writing, for me, is joy. I like putting thoughts down and sending them into other people's heads. If something I wrote plants a new idea in someone, or opens a conversation I wouldn't have had otherwise, that's the whole point. That's how my world widens.

I'm not giving that up because a detector got nervous. I'm going to keep writing — with the tools that make me sharper, grounded in the person I already am.

Sound like yourself. That's the whole job.
