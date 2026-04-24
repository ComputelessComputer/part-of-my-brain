---
title: Finished software is dead software
created_at: 2026-04-23
updated_at: 2026-04-23
published: true
tags:
  - engineering
lang: en
description: No software is ever finished. Trying to perfect it before shipping is slower than shipping and fixing what actually breaks.
---
Every piece of software you've ever loved was broken when it shipped. Yours will be too.

There's no static version of software. No final build, no finished product. Every piece of working code needs a human on the other side — patching dependencies, fixing edge cases, adapting to the user who used it in a way you never pictured. The world keeps changing. Your software changes with it or it dies.

There are two ways to plan around this. Think upfront, build a foundation that holds. Or iterate as fast as possible and let reality tell you what the foundation should be. Garry Tan's [gstack](https://github.com/garrytan/gstack) is the clean version of the first — 23 structured roles reviewing every step from spec to QA. Peter Steinberger built [OpenClaw](https://steipete.me/) the other way. The first version took him an hour. Both are planning.

I'm in Steinberger's camp. It's the uncomfortable one: ship something rough, use it, fix what actually breaks. Not what you imagined would break. What does.

When I built [Philo](https://philo.so), I didn't plan it. I needed daily notes that Claude Code could read and write to without an API or SDK, so I wrote the smallest thing that did that, used it every day, and patched whatever annoyed me. Two weeks from scratch to a version I lived in.

Three weeks in I was fixing things I never would have written on a design doc — the always-on-top mode needed to fade when the window wasn't active, the global search needed to replace the whole view instead of hover. Trivial bugs. Only visible from inside the app. My cofounder [Yujong](cofounder) was astonished at the speed. What surprised him more was that it worked.

It worked *because* I shipped it broken. Every bug I hit was a bug I would have hit anyway, just later. Shipping first meant hitting them while they were still cheap.

The version where I tried to get it right the first time doesn't exist, but I can describe it: a month of whiteboarding cases I thought mattered, then another month discovering I'd guessed wrong about most of them. We spent months at Char believing flat files were the right storage layer. No whiteboard would have told us otherwise. Actually running Char on them did.

SpaceX failed three times before [Falcon 1](https://en.wikipedia.org/wiki/Falcon_1) reached orbit in 2008. Not because they were careless. Because the only way to learn what reality does to your design is to put the design in front of reality. Software blows up cheaper than any rocket.

Shipping rough has costs. In April we [[essays/lessons-from-shipping|pulled local transcription]] before the replacement was stable, and we lost 200 of our earliest users. That's the tax. I'd still take it over six months of planning that shipped nothing.

None of this is permission to be sloppy. The opposite. Accepting that nothing is ever finished is what *makes* sustained attention possible. You ship, and then you care. Forever. Every user report, every dependency update — that's the job, not an interruption from it.

Ship it. Then stay.
