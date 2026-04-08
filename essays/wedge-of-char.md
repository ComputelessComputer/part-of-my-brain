---
title: What Char is optimizing for
created_at: 2026-04-09
updated_at: 2026-04-09
published: false
lang: en
description: We built a local-first meeting notetaker and then started making decisions that confused people who came for exactly that. Here's why.
---
A few days after I published [the last essay](https://johnjeong.com/essays/future-of-char), our Discord lit up. We'd quietly swapped our transcription provider — argmax parakeet to cactus's whisper v3 turbo — without a working replacement in hand. We also removed the live transcript view. People who had paid for months of Char, who had specifically chosen it because of on-device, no-cloud-audio promises, were rightfully pissed.

One person summed it up well: *"You are essentially killing all local features."*

That's not what we intended. But intentions don't matter when the outcome is a broken product with a description that still reads *"private, on-device AI notepad that enhances your own notes — without bots, cloud recording, or meeting intrusion."*

So let me be direct about what happened, why we made these calls, and what we're actually optimizing for.

---

### The mistakes, plainly

We replaced a working STT with one that wasn't working yet. That was bad judgment — full stop. There was no good reason not to keep argmax parakeet live while cactus stabilized. We moved too fast and created a week of broken transcription for users who depend on the app daily. We're sorry.

We also removed the live transcript view without a feature toggle. The reason was real — some hardware couldn't handle real-time on-device inference without degrading — but the solution was lazy. A settings toggle solves that. Stripping the feature entirely was the wrong call, and we'll bring it back once the new provider stabilizes.

Those were execution mistakes. What I want to address separately is the *strategic* shift underneath them — because that's not a mistake, and I think it deserves a real explanation.

---

### What we're not building

When I wrote the last essay, I said the wedge wasn't meeting notetaking. Someone pushed back in the Discord:

> "Your wedge into becoming the executive assistant for founders IS to be the best local meeting transcription tool. Without it, I would use an alternative path."

It's a fair argument. And I thought about it seriously.

Here's where I landed: there's a version of Char where we spend the next two years optimizing real-time on-device transcription across every chipset, every OS version, every audio configuration. It's a real product. It's useful. And I think tools like Meetily are better positioned to win that fight than we are — not because we can't build it, but because it's not what we're uniquely motivated to obsess over.

Real-time local transcription solves a specific problem: you want to see words appear on screen during your meeting. The honest use case, per our research, is mostly reassurance that the app is listening — and catching up on parts of the meeting you zoned out of. That's real value. It's just not the value that unlocks the bigger thing we're building toward.

What actually matters is: *after the meeting ends, does Char know what happened well enough to do something useful with it?*

Batch processing — transcribing after the call is over — produces more accurate transcripts than real-time on-device inference on most hardware. It's quieter, less error-prone, and fits into a workflow where the important stuff happens post-meeting anyway. That's the foundation we need.

---

### Local-first still means something

We're not abandoning on-device transcription. It ships free, it always will, and the premise — that you can use Char without sending your audio to a cloud server — remains true.

What changed is where we're allocating engineering attention. The cloud models unlocked by the paid plan are not a replacement for on-device; they're a different layer. Cloud gives us memory. Shared context. The ability to connect what happened in Tuesday's meeting to what someone asked in Thursday's. On-device gives you privacy and zero latency. Both matter. They serve different people in different moments.

For people who need a stable, reliable, real-time, private transcription experience above all else: Char is not your best option right now. I'd rather say that clearly than have you stay on a paid plan waiting for something we're not prioritizing.

For people who care about what flows *from* a meeting — tasks, decisions, context — we're building exactly for you.

---

### How we're prioritizing

The vision I laid out in the last essay — EA, Chief of Staff, COO — is directionally right. But vision without a sequencing framework is just a mood board. Here's how we're actually thinking about what ships when:

**First: the foundation has to work.** Sync is shipping in April. Folders after we migrate back to SQLite. These aren't exciting announcements, but broken or missing infrastructure makes every feature on top of it worse. We're paying down that debt before adding surface area.

**Second: the daily note has to become the gravity well.** The daily note is where context accumulates — meeting notes, captured thoughts, surfaced tasks. If that's not compelling on its own, nothing downstream works. We're treating the daily note as the product right now, not a feature inside the product.

**Third: agentic handoffs.** The Chief of Staff moment — where Char routes a spec to Cursor, flags a decision to a co-founder, drafts an email — requires the first two to be stable. We're not rushing it. When we ship it, it has to actually work.

What's explicitly deprioritized: more transcription providers, advanced privacy configurations, integrations with tools we haven't validated matter to our users. We'll revisit, but not now.

---

### The wedge

So what's the wedge?

Not real-time local transcription. Not privacy as a feature. Not being a cheaper Granola.

The wedge is the daily note — and the claim that Char can be the thing you open at the start of your day and close at the end, with your whole context accumulated inside it. Meetings feed into it. Tasks surface from it. Over time, it becomes your working memory.

That's the promise we're building toward. It's a harder thing to explain on a landing page than "on-device notetaker." But it's the only version of Char worth building.

We made some fumbles making this transition clear. The product got messy in a moment where clarity mattered most. I own that. What I'm trying to do now is make sure the direction is visible — not just in an essay, but in every decision we make about what ships and what waits.
