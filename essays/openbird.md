---
title: I Built an Open Source Alternative to Littlebird
created_at: 2026-04-01
updated_at: 2026-04-01
published: true
tags:
  - engineering
  - memory
lang: en
description: Why I built Openbird, a local-first activity journal that captures your day through accessibility data with no cloud, no screenshots, no lock-in.
---
I built an open source activity journal for macOS.

Most "personal AI" tools want your screenshots, your keystrokes, your clipboard. They capture everything and send it somewhere. I wanted something that felt less like surveillance and more like a journal that writes itself.

[Openbird](https://openbird.vercel.app) watches what app is in front, what window is active, what URLs you visit. It uses macOS accessibility APIs, nothing else. No screenshots, no key events, no clipboard, no passwords. Then it summarizes your day.

Everything stays on your machine. One SQLite file in `~/Library/Application Support/Openbird/`. You can pause capture, exclude apps, delete data by timeframe. There's no account, no cloud sync, nothing leaves your Mac.

It works with whatever model you want. Ollama, LM Studio, any OpenAI-compatible endpoint. Bring your own inference.

I built Openbird as a proof-of-concept for something bigger. I want [Char](https://char.com) to have a personal-context layer, something that knows what you've been working on and can surface relevant context when you need it. But that layer needs to be trustworthy first. Openbird is me figuring out what trustworthy looks like.

The hard part isn't the tech. It's deciding what not to capture. Every piece of data you collect is a liability. I'd rather start with too little and add more when there's a clear reason than start with everything and hope people trust you.
