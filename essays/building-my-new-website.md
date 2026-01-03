---
title: "Building This Website"
created_at: 2026-01-02
published: true
tags: [meta, engineering]
lang: en
description: "Building a file-based personal website using Obsidian as a CMS, Git for versioning, and a philosophy that files endure while interfaces change."
---
I Built My Life on Files

  

I rebuilt my website, but what I really rebuilt was the system behind how I think, write, and leave traces of my life on the web.

  

This is not a post about frameworks or tech stacks. It is about choosing a foundation that ages well. One that works for humans today and machines tomorrow.

  

The Problem

  

I wanted a simple setup.

  

I wanted to write in tools I already use every day.

I wanted to publish selectively without friction.

I wanted people to respond without me running a database.

And I wanted everything to be durable, inspectable, and owned.

  

Most personal websites solve publishing. Very few solve living with your thoughts.

  

Interfaces Are Temporary. Files Are Durable.

  

Over the years, I tried many note taking apps. Obsidian, Reflect, Roam, Logseq, Apple Notes, and others. They are all good in different ways. But over time, one thing became obvious.

  

Interfaces change. Files endure.

  

Markdown based, file based systems work because they separate data from views. When an interface starts to feel limiting, you do not have to migrate your brain. You just change how you look at the same files.

  

Obsidian is a great product. But when I want to view daily notes in a strict timeline, it is not the best tool. There are probably plugins that solve this, but at some point it is easier to use software that was designed for that mode of thinking from the beginning.

  

That is when I stopped looking for a single perfect workspace.

  

Instead, I optimized for a stable data layer and multiple specialized interfaces.

  

File System Is the Cortex

  

I truly believe file based systems are fundamental in the AI era.

  

Most modern coding agents work well not because they are magical, but because the environments they operate in are simple. Code lives in files. Agents navigate those files using basic tools like ls, find, grep, and cat. They scan directories, extract context, and reason step by step.

  

The intelligence emerges because the substrate is legible.

  

When your thoughts live in files, plain text, predictable folders, you create an environment that both humans and machines can understand. The file system becomes the cortex. Interfaces are just different ways of viewing it.

  

This is why file based systems are not nostalgia. They are future proofing.

  

Separation Is Clarity, Not Fragmentation

  

In theory, one unified app for everything sounds elegant. In practice, different kinds of thinking benefit from different environments.

  

You do not do everything on one desk.

  

You might write at a clean desk with just a laptop and a notebook. But if you are building something physical, you move to a workbench in the garage. You do not want hammers mixed with paintbrushes.

  

That is how I treat my tools.

  

I use Logseq for daily logs and timeline style journaling.

I use Obsidian for long form thinking like essays, inspirations, and lessons.

I use Hyprnote for meeting notes.

  

All of them operate on files. That is the invariant.

  

By separating interfaces while keeping the data unified, I get clarity without lock in.

  

Some Underrated Benefits of Files

  

There are also very practical reasons this setup works well.

  

First, it is local first.

  

File based systems run locally by default, which makes them fast. Notes open instantly. There is no network round trip just to read your own thoughts. No waiting for sync to finish before you can think. For note taking, this matters more than people admit.

  

Second, local first does not mean fragile.

  

You cannot always trust yourself to back things up perfectly. That is the advantage of being digital. Copies are cheap.

  

When your life lives as files, backup becomes trivial.

  

I use Git for this. Every meaningful change is versioned. Every mistake is recoverable. Every file exists in more than one place.

  

Using GitHub is a bet on durability. I am betting that Microsoft will not disappear in the next hundred years. That feels like a safe bet.

  

Do I love all of their products. Not really. But the company is not going to vanish quietly, and that matters more than aesthetics when you think in decades.

  

The point is not GitHub specifically. The point is that file based systems let you choose your redundancy strategy. You can mirror, fork, archive, or move everything somewhere else at any time.

  

Local first for speed. Distributed copies for safety.

  

That combination is hard to beat.

  

Obsidian as a CMS

  

Obsidian has effectively become my CMS.

  

I use it to write essays, document what inspired me, and keep track of books and ideas I have learned from. Everything lives in a public vault with a simple folder structure.

  

Essays are ideas I am confident enough to stand behind.

Journals are daily logs and thinking in motion.

Inspirations are talks, podcasts, and videos that shaped me.

Lessons are distilled knowledge from books and courses.

  

Publishing is controlled entirely through frontmatter.

  

If something is not ready, it is marked as published false. When it is ready, it becomes part of the site automatically. Journals are always public by default.

  

Writing and publishing are no longer separate actions. Publishing is just a side effect of writing.

  

The Architecture

  

The site itself is intentionally boring.

  

There are two repositories.

  

One is my public Obsidian vault.

The other is the website that renders it.

  

The vault is pulled into the site using a git submodule. When I push changes to either repository, the site rebuilds.

  

Publishing is git push.

  

There is no database. No admin panel. No CMS UI to maintain.

  

Comments Without a Database

  

For comments, I use GitHub Discussions through Giscus.

  

When someone comments on an essay, it creates a discussion in the vault repository. Each content type maps to its own category. Authentication, moderation, and spam resistance are handled by GitHub.

  

The tradeoff is simple. Commenters need a GitHub account. I am fine with that.

  

I also added a Questions category. The site has a form that submits directly to Discussions. It is effectively a self hosted AMA without infrastructure.

  

Why This Works

  

This setup works because every layer does one job well.

  

Obsidian is my CMS. I write where I already think.

Git is my memory. Version history, backup, and truth.

Astro is my renderer. Fast, static, markdown native.

GitHub is my community layer. Comments and questions.

  

Everything is just files and a static site generator.

  

But more importantly, this setup reflects who I am.

  

I wanted my website to be a transparent archive of my life. Not optimized for growth. Not trapped inside a platform. Not dependent on a company staying alive.

  

If I die, this is the place where my thoughts remain.

  

Not on Twitter.

Not inside a closed database.

  

On the web. As files I actually own.