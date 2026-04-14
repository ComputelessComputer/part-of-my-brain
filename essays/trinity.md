---
title: The Trinity of a Startup
created_at: 2026-04-14
updated_at: 2026-04-14
published: true
tags:
  - startup
  - char
lang: en
description: I was a priest who didn't believe in his own Bible.
---
Every startup has three parties: the founders, the product, and the customers. All three have to be *philosophically aligned*. If any one is off — even slightly — the team burns out, the product doesn't hit, or people just leave.

I've been dealing with this for the past year.

## The religion analogy

A startup is like building a religion.

As a Catholic, I go to church every Sunday. There's the priest — the founder. There's the Bible — the product. And there's the worshippers — the customers.

When all three resonate, a community forms naturally. Worshippers talk about the Bible. They trust the priest. They keep coming back every Sunday. It stops being shamanism and becomes a real movement.

When it doesn't work, you're a priest who doesn't believe in his own Bible.

![](john_jeong_8-bit_pixel_art_a_small_warmly_lit_church_interior_8f22fccf-e356-4c4d-adfd-16cb72617b2f_3.png)
## Six months of misalignment

I [[essays/post-yc-slump|wrote about the post-YC slump]] before. When we first started Hyprnote, it was a project. And for the first six months — April to October 2025 — there was a deep misalignment inside the founding team.

Yujong and I couldn't agree on what the product should be. That stalled us completely.

The cruel irony: there were worshippers showing up to church every Sunday — actual users trying to use and pay for our product. A Bible that accidentally resonated with people. But the priests didn't know what the hell was going on, so we couldn't lead the congregation.

During those six months, I kept arguing that local-first and on-device models were nice-to-haves. The most important thing for a productivity app is *productivity itself* — not privacy, not architecture purity.

But we were too caught up thinking about enterprise software without ever building software useful for individuals. We were thinking too hard about structural moats — how to not get crushed by OpenAI or Granola — instead of just growing.

As I [[essays/future-of-char|wrote in "Future of Char"]], growth matters more than strategy at this stage. The turning point was hearing PG talk in Mountain View about how growth tops everything. That's when I could finally persuade Yujong that local-first-only was not the way.

## Losing faith in the Bible

Throughout that year, I consistently thought: a meeting note-taker is a feature, not a product. You can build one to production grade in a couple of weeks. The codebase can be slop and it'll still work. It's just too easy.

I didn't buy it — not just the business model, but the whole premise. A meeting is just one node inside a company where decisions happen. You could listen to Slack too — that's where async decisions are made. You could hook up workflows, integrations, everything.

Then we did user interviews. Our existing users saw us as a *free transcription tool* — open source, cared about craftsmanship, reasonable quality. I was grateful they tried us. But I also thought: we're fucked. We were building "open-source Granola" but people saw us as "free on-device transcription". That gap is fatal.

And the deeper I went — experimenting with [[essays/philo|Philo]], [[essays/openbird|Openbird]], [[essays/fs-cli-is-the-future|aipm]], [Arx](https://github.com/ComputelessComputer/arx) — the more I believed you have to focus on individuals to make something truly great. I gradually stopped believing in the concept of open-source Granola because I stopped believing in what Granola itself represented.

## You have to know your worshippers

Defining an ICP isn't about selling. It's about whether you actually give a shit about these people's problems.

If you don't, you can't resonate with them. Logic alone is shallow — it's what you lay out to sound sane. Anyone can nod along to a sane argument. What actually matters is understanding the emotional stuff, the nitty-gritty of someone's daily pain.

I wasn't aligned with our customers. I had access to every model, no restrictions, juicing maximum productivity. I was building a privacy-first product while being the least privacy-focused person who would use it — and still the most privacy-centric person on the team.

I never went to big tech. I never lived the life our users lived. I was preaching to a congregation I'd never sat in.

## The pivot

Starting from October, we decided to build what we actually believed in. By February 2026, after experimenting with all those products, I reached a conclusion: we shouldn't just capture context. [[essays/wedge-of-char|We need to utilize it]]. There's more context to capture beyond meetings. And on-device can't support all of that right now — the hardware and models aren't there yet.

So we pivoted. The Discord blew up. Users were upset. Many left.

Frankly, I'm fine with that. The priest, the Bible, and the worshippers were all pointing in different directions — so every new chapter we wrote went unread. [[essays/lessons-from-shipping|We'd been shipping constantly]] and it didn't matter because the foundation was broken.

A pivot means the congregation leaves — or you leave them. The most graceful thing I could do was build Unsigned Char in a week. An on-device AI meeting note-taker, bot-free, same form factor, focused purely as a utility tool. A parting gift for the old worshippers.

## Where we are now

There hasn't been a moment in our startup journey where we've been closer to our product. [[essays/openbird|Openbird]], [[essays/philo|Philo]] — these features now integrate into Char for reasons that actually make sense to us. We have a constitution now. When we were building Hyprnote, we didn't.

But the worshippers aren't aligned yet. We need to find the congregation — people who believe in what we believe.

You can't fake the trinity. If the priest doesn't believe, the Bible is hollow. If the Bible is hollow, the worshippers sense it.

All three have to click. We're two-thirds of the way there. The last third is the hardest.