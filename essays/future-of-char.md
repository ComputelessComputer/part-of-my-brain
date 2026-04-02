---
title: Char is not a meeting notetaker
created_at: 2026-03-29
updated_at: 2026-04-01
published: true
lang: en
description: The real question was never how you capture a meeting. It was what happens to everything that flows from it.
---

We launched Char a year ago as a meeting notetaker. I've come to believe that framing was too small.

The real question was never *how do you capture a meeting?* It was: *what happens to all the intent, context, and decisions that meetings produce — and who is responsible for carrying them forward?*

That's the problem Char is now built to solve.

We got into YC, finished the batch, and raised our seed. But more importantly, we spent a year making nearly every mistake available to an early-stage founder — and coming out the other side with a clear point of view. Here's what that looks like.

---
### What I believe

These four things won't change for the next 10 years.

#### 1. Taste is the last moat

AI has widened the gap between people with craft and people without it. Those without it are converging — LLMs trend toward a statistical average, and without taste, there's no impulse to push further. Great work still requires someone with a strong point of view. That gap is only growing.

#### 2. Preference is the forcing function for human collaboration

Organizations will shrink. AI resolves inefficiency faster than any headcount can. But I've learned that AI works best with a human in the loop — not because it can't execute, but because doing something *great* requires sustained attention across every domain simultaneously: design, engineering, marketing, sales. No one can hold all of it. People have natural preferences, and that's what drives collaboration. It doesn't disappear with AI — it becomes more deliberate.

#### 3. Everyone is becoming a manager

Traditional orgs were information pipelines: decisions flowed down, Individual Contributors (ICs) executed on behalf of managers. That model is breaking. Today, everyone is running a fleet of AI agents to get their work done. Whether they realize it or not, everyone is becoming a manager.

#### 4. Humans are naturally poor at managing complexity

Entropy always increases. Even the most senior people in an org have someone managing things for them — a Chief of Staff, an Executive Assistant. The higher the expected output, the more support is required. If everyone is now managing AI agents, the question becomes: *who manages the managers?*

That last question is the one Char is built to answer.

---
### How we got here

#### April 2025: Building in the dark

We started Hyprnote in December 2024. AI was still weak enough at coding that we built everything ourselves — including a Rust-based audio pipeline that essentially didn't exist in open source yet. That was hard, but technical challenges have answers. What we struggled with was harder: we didn't know what we were building *for*.

The question we kept circling was whether to bet on *open source* or *on-device transcription*. Both were real advantages. We couldn't decide, so we kept both alive. That was the first mistake.

#### May 2025: A signal from the market — chased too fast

After a [successful launch on Reddit](https://www.reddit.com/r/LocalLLaMA/comments/1k3fdqa/i_spent_5_months_building_an_open_source_ai_note/) in April, something interesting happened: directors and senior managers started reaching out. They wanted a safe AI notetaker. Many employees at larger companies couldn't use existing tools due to data policies. We saw an opportunity to get inside the doors of large enterprises.

But the open source vs. on-device question was still unresolved. We told ourselves we could do both.

#### YC: The wrong bet, executed poorly

We applied to YC with the enterprise thesis. Our first instinct was to reach out to "potential" leads — which was the wrong move entirely. We were targeting a segment we'd never validated, throwing darts in the air while blindfolded.

We pivoted to bottom-up sales, identifying existing users and having real conversations. That was harder than expected — we'd launched with license keys, so most users were anonymous. We had almost no contact information to work with.

And the enterprise requirements kept fragmenting. Every conversation surfaced a different priority: privacy, security, data sovereignty, all-party consent laws. Each was a real concern. Each pointed somewhere different.

We pushed hard to generate traction and saw meaningful adoption inside Fortune 500 companies. But we never got clear on direction. In hindsight, the pressure of demo day was pulling us toward premature focus. Since then, I've built in structured thinking time — it's made a real difference.

#### October 2025: The decision

Yujong and I sat down in Seoul after the batch ended. We'd been chasing enterprise for three months. We laid out what we actually knew versus what we were hoping was true.

We cut enterprise.

The reasoning was simple in retrospect: enterprise sales for AI notetakers runs entirely on end-user adoption. You can't skip bottom-up and go straight to the top. We'd been trying to. The only path to enterprise was through individual users first — if and only if we cracked that, we'd have a foundation for anything else.

#### December 2025: Rebuild — and listen to the data

We launched a new version quietly, with no announcement. We wanted to build without noise and let the data tell us what was actually happening.

For context — this retention chart shows cohorts of users who were active (performed `note_enhanced`) in their first week and returned to do it over and over again.

###### 1. High-intent users retained exceptionally well

Our activation funnel was nearly nonexistent at launch, which meant only the most motivated users made it through. The result was record-high retention in that early cohort.

![](when-activation-sucked.jpg)

###### 2. A hiring post surfaced the wrong users

Inflows from our designer job post brought in curious but low-intent users. They churned quickly — expected, but useful to see clearly in the data.

![](when-we-were-hiring.jpg)

###### 3. Better activation meant a broader, more demanding user base

After improving the activation funnel significantly, more users reached their first meeting note. But more generic users also got through, and they needed more feature completeness. [We shipped hard.](https://char.com/changelog/)

![](when-we-improved-activation.jpg)

###### 4. Pricing clarified who our real users were

We experimented with our pricing, moving from $8 to $25/month. Retention dropped from 56.9% to 48.5%. We recovered quickly as the product improved. During this period, I ran around 20–30 user interviews and found two distinct groups: people with sparse meeting schedules and people with back-to-backs. We introduced a Lite plan at $8 to serve both.

![](when-we-announced-price-update-and-migration-kicked-in.jpg)

#### March 2026: The opening

Granola recently [raised at a ~$1B valuation](https://www.forbes.com/sites/iainmartin/2026/01/30/vcs-favorite-note-taking-app-granola-in-talks-to-hit-1-billion-valuation/) and is moving upmarket toward enterprise. I think that's a gift.

For the past few months I've been building adjacent tools and dogfooding them every day — a task manager, a daily notes app, an automatic activity log, an inbox cleaner. The pattern I kept running into: each tool worked in isolation, but none of them had *context over time*. The missing layer wasn't another tool. It was something that connected all of them, with memory, continuously.

I also came back to something I'd underestimated: being a first mover in a category matters — not for market share, but because a new paradigm, once experienced, gets imprinted. We needed to stop being a better Granola and start being something Granola couldn't become.

The natural question at this point is: **what's the new paradigm that Char has to offer and how will it stand out?**

---
### Char 1.1 — The command center for founders

Think back to belief #4: humans are naturally poor at managing complexity. Every high-output person has someone managing things for them. Char is going to be that for founders.

###### Executive Assistant

The daily note is going to become our killer feature — building Philo made me genuinely bullish about this, and frankly I'd been thinking about it since last year.

![](Pasted%20image%2020260401165943.png)

A daily note that evolves throughout your day is like having an Executive Assistant, in a very subtle way.

![](Pasted%20image%2020260401175215.png)

When you finish a meeting, action items surface directly in your daily note. You no longer need to track them somewhere else — and it's where you capture everything that's on your mind. Over time, Char becomes your memory for everything.

This is the first step.

###### Chief of Staff

In the future, not only will tasks become things you shouldn't have to execute — you shouldn't have to manage them either.

Daily notes are a timeline-based way of constructing episodic memory. I'm confident that triaging tasks will be far easier with rich context — I've learned this while building aipm and trialing tools like Modem. They fall short when they don't have an evolving context, because they only echo loud signals which are often noise.

Imagine this. You finish a difficult product meeting. Three action items surface in your daily note: a spec to write, a design decision to unblock, an email to send. You don't touch any of them. Char has enough context from the conversation to route the spec to Cursor, flag the design decision to your co-founder's daily note, and draft the email for your review. By the time you're in your next meeting, the work is already in motion.

![](Pasted%20image%2020260401180653.png)

###### Chief Operating Officer

The full picture is still coming together — but the direction is clear. When everyone inside a team has their own daily note, those notes become a shared operating layer: context flows between people automatically, decisions leave a trail, and nothing falls through the cracks because the system remembers even when people don't.

That's the company we're building.

![](Pasted%20image%2020260401181308.png)
