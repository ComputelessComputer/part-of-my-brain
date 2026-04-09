---
title: We shipped 21 versions and broke trust
created_at: 2026-04-09
updated_at: 2026-04-09
published: true
lang: en
description: We moved fast for three months and lost our earliest users in the process. Five mistakes I won't repeat.
---
Between January and April we shipped 21 versions of Char. Rebuilt the storage layer, renamed the product, swapped transcription providers, redesigned the editor, added three calendar integrations. Most of it worked. Five things didn't.

---

### 1. Swapping the storage layer mid-flight

**What we did.** In January we replaced our SQLite storage with JSON and markdown-based persisters. I was genuinely convicted about this — I [wrote a whole essay](https://johnjeong.com/essays/fs-cli-is-the-future) arguing that the file system and CLI are the right interface for AI-native products. I'd been building [Philo](https://philo.so), an [open-source daily notes app](https://johnjeong.com/essays/oss-alternative-logseq), with plain markdown files, and Claude Code could read and write to it with zero setup. No API, no auth, no SDK. That experience made me believe flat files were right for Char too.

**What went wrong.** Char isn't a vault of markdown files. It's an application with structured data, relationships between entities, and operations that need to be atomic. Once you have a comprehensive CRUD layer that abstracts the app, you don't need the file system to be the source of truth. The abstraction *is* the interface. Files just add indirection.

Folders got blocked. Search was slower. Sync was harder to reason about. Yujong and I circled this dependency in every product session since March — by March 31st we'd identified the SQLite migration as the single largest blocker to everything we wanted to build. We're now doing the migration we deferred, except with more data, more users, and more surface area to break.

**What I'd do differently.** Timebox it. Two months on flat files to learn the shape of the data, then migrate back. Instead we let it drift and it became load-bearing. When you do something deliberately temporary, write down when it ends.

---

### 2. Removing Argmax without a stable replacement

**What we did.** On April 1st we removed Argmax — our working local transcription provider — and replaced it with Cactus, which wasn't stable yet. Also removed the live transcript view. No announcement. No toggle. No fallback.

**What went wrong.** This wasn't purely an execution mistake. Yujong and I had been moving toward this for weeks. On March 27th we agreed that transcription alone couldn't justify our pricing. On April 3rd we discussed shifting to batch processing. On April 4th, when complaints came in, we agreed to deprioritize — the affected users were largely non-paying.

That was wrong. Free users are your distribution. They're the ones posting on Reddit and recommending you in Discord servers you've never heard of. Dismissing their pain because they weren't paying was short-sighted.

One user: *"You are essentially killing all local features. First you remove the only working local STT without providing an alternative and next you remove live transcript."*

Another: *"That's also not how enterprise grade software shipment works — given your new focus."* That stung because we'd been talking about moving upmarket while shipping like we had no users.

We fixed it in v1.0.21 a week later. Parakeet V3 and Whisper Small are back, batch-only.

**What I'd do differently.** Ship the new thing alongside the old thing. Both providers in settings. Gradual migration, not a one-shot swap. Announce before you break — a simple Discord message would have changed the entire dynamic. And talk to users before removing something they use, not after.

I've since added a rule: any change that removes or degrades a feature gets announced in Discord at least 48 hours before shipping.

---

### 3. No communication rhythm

**What we did.** February was our most feature-dense month — full-text search, redesigned calendar, chat panel, backlink mentions, local STT, custom vocabulary — all shipped back to back without changelog posts or Discord context.

**What went wrong.** Users didn't know what was new or what might break. Features landed silently. The velocity felt productive internally but created confusion externally.

**What I'd do differently.** A weekly Discord post — "here's what shipped, here's what's next" — would have taken 15 minutes and turned confused users into testers.

We'd never sent educational content to existing users. Not once. Even after the STT blowup, our plan was "respond to the Discord thread, post an announcement, put it in the newsletter." All damage control. No system. I'm fixing this now — but it's not fixed yet.

---

### 4. Renaming without updating the positioning

**What we did.** In March we renamed from Hyprnote to Char — Hyprnote described a feature, Char describes a role.

**What went wrong.** Google still showed *"Char is a private, on-device AI notepad that enhances your own notes — without bots, cloud recording, or meeting intrusion."* Users arrived expecting one product and found another. One called it out: *"I downloaded on the premise of on device transcription and no sending audio files to the cloud, and had signed up under a paid plan for many months. I actually don't understand what's supposed to be private anymore?"*

**What I'd do differently.** A rename is a repositioning. Update every surface — app store, meta tags, landing page, social bios — in the same release. If the positioning has changed, own it loudly.

---

### 5. Not migrating 0.0.84 users

**What we did.** When we shipped the 1.0 rewrite, we left users on the old version behind. No migration path, no nudge, no guided transition.

**What went wrong.** Up to 200 daily active users churned out instead of upgrading. Our earliest adopters — people who'd stuck around through the roughest versions. Lost to neglect, not to a bad product.

**What I'd do differently.** Migration is a feature. In-app prompts, a "here's what's new" flow, even just an email.

---

### The pattern

All five are the same mistake. We were building fast and not talking to the people using what we built.

The best version of an early-stage company is when the founder, the product, and the users are all pointed in the same direction. When that's working, users recruit for you. They forgive bugs because they trust the direction. I wanted that for Char and I was breaking it without realizing.

Broken STT, removed features, stale positioning, 200 abandoned users — that's a pattern that tells your community you're building for yourself. Once people feel that, they leave. Not angrily. They just stop opening the app.

I'm not going to start shipping slowly. But I am going to communicate before I break things and treat our Discord like collaborators instead of an audience.
