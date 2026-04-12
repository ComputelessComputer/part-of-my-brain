---
title: Customize your terminal
created_at: 2026-02-05
updated_at: 2026-04-12
published: true
tags:
  - engineering
lang: en
description: Your terminal is the most-opened app you have. Here's why it should feel like yours.
---
Engineers — you open your terminal more than anything else. More than Slack, more than your browser. You live there. Mine still looked like it came out of the box two years in.

That bothered me more than it should have. So I fixed it.

---

There are a few layers to this. Your `.zshrc` is the foundation — aliases, prompt shape, the small things that compound. Oh My Zsh handles the structure if you don't want to start from scratch. Above that is the emulator itself: Ghostty is fast and native, Warp rethinks the whole thing with blocks and a command palette. I use both. Ghostty for everything, Warp when I want its UI.

Then there's the stuff that's purely aesthetic and entirely worth doing. Mine prints an ASCII image and my system info every time I open a new window. Takes 80ms. Gives me nothing. I love it.

![[assets/Pasted image 20260406070647.png]]

My dotfiles are [here](https://gist.github.com/ComputelessComputer/ebfb3d5729f51f3104afe1bb78142504).

---

No one touches your terminal but you. It's the one corner of your machine that's completely yours. Most people never bother making it feel that way. I think that's a mistake.
