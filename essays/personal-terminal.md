---
title: Customize your terminal
created_at: 2026-02-05
updated_at: 2026-04-06
published: false
lang: en
description: Your terminal is the most-opened app you have. Here's why it should feel like yours.
---

There's a running joke that engineers spend more time configuring their tools than actually using them. I think that joke misses the point entirely.

Your terminal is the one app you open more than anything else. More than Slack, more than your browser, more than your IDE. It's where you ship things, debug things, and occasionally watch a build fail for the fourth time in a row. You live there. So why does it look like it just came out of the box?

## The case for making it yours

Most engineers inherit a terminal setup. They install the OS, open Terminal.app, and just... start typing. The defaults are fine. They work. But "fine" and "yours" are very different things.

When a space feels personal, you take pride in it. You notice when something's off, you care about keeping it clean, and — maybe most importantly — you actually enjoy being there. That's not a small thing when you're spending hours a day in a single window.

The terminal is also uniquely yours in a way that almost nothing else is. Your text editor has opinions. Your browser has extensions fighting over it. Your Notion workspace has pages your teammates touched. But your terminal? Nobody goes in there. It's the one corner of your machine that's entirely under your control.

## The layers of customization

Personalizing your terminal happens at a few different levels, and you don't have to go deep on all of them.

**Shell configuration** is the foundation. Your `.zshrc` (or `.bashrc`) controls your aliases, environment variables, functions, and prompt. Even small things here — a short alias for a command you run fifty times a day, a prompt that shows your git branch — compound over time. Oh My Zsh is a popular framework that layers on top of this with plugins and themes, and it's a good starting point if you want structure without starting from scratch.

**Your terminal emulator** is the next layer up. This is the actual app — the window, the font rendering, the tabs, the feel. The default Terminal.app on macOS is stable and capable, but it's also clearly not trying to impress you. Alternatives like [Ghostty](https://ghostty.org) and [Warp](https://www.warp.dev) have rethought what a terminal can be. Ghostty is fast, native, and endlessly configurable. Warp leans into modern UX — block-based output, built-in AI, a command palette — which makes it feel less like a relic and more like a tool built for 2026.

**Aesthetics** are the final layer, and arguably the most personal. Your color scheme, your font, your prompt shape, and yes — things like [neofetch](https://github.com/dylanaraps/neofetch) or its faster successor [fastfetch](https://github.com/fastfetch-cli/fastfetch), which prints a system summary with ASCII art when you open a new shell. It's entirely useless and completely worth doing.

## My setup

I run Ghostty as my daily driver with Warp open alongside it for longer-running tasks where its block UI is useful. My shell config has grown slowly over a few years — mostly aliases and a handful of functions I've forgotten I wrote until I accidentally type their name somewhere else.

The thing I'm most attached to is my neofetch config. Mine renders a custom ASCII image alongside my system info every time I open a new terminal window. It takes about 80ms and gives me nothing practical. I love it.

![[assets/Pasted image 20260406070647.png]]

My full dotfiles are [here](https://gist.github.com/ComputelessComputer/ebfb3d5729f51f3104afe1bb78142504) if you want somewhere to start.

## Your terminal, your rules

I'm not going to tell you which terminal to use or what your prompt should look like. That's the whole point — there's no right answer, only what feels right to you.

What I will say is that the effort is worth it. Not because a custom terminal makes you a better engineer (it doesn't), but because it makes the place you work feel like *yours*. No one can touch it. No one can mess with it. It's your space, and you can make it whatever you want.

That's rarer than it sounds. Make the most of it.
