---
title: Char is your context aggregator
created_at: 2026-06-01
updated_at: 2026-06-01
published: false
tags:
  - startup
lang: en
description: A meeting notetaker captures one room. Char captures every surface — meetings, screen, integrations, notes — and turns the checkboxes you write into work that gets done.
---

Two months ago I wrote that [the wedge for Char is the daily note](wedge-of-char). The daily note is still the surface. But after a month of customer-discovery interviews, I have a better word for what's underneath.

Char is a context aggregator. It's the only thing that can hold the work AI is supposed to do for you.

---

#### The shape of the problem

I spent May talking to twenty founders about how they actually run their day. The thing I expected to find — that founders live in Linear, or Notion, or Asana — was wrong.

The modal task surface for a founder is Apple Notes.

Not Linear. Not Notion. Not Things or Todoist or any of the apps I've been benchmarking against. Plain text, in Apple Notes, on a phone. Abhay at Frizzle keeps one called "Frizzle Growth." Madhav at AirCaps keeps several. I keep mine in there too, even after building two notes apps. So does Jesse at Bidflow, except he keeps his in his head — which is its own answer.

The reason is obvious once you see it. Apple Notes is the only surface that doesn't punish you for writing something down. There's no schema. No project. No tag. No \"is this a task or a note?\" decision. You open it, you type, you close it. The cost of capture is zero.

Every \"better\" tool I've ever used has been worse at exactly this. Linear wants a team and a status. Notion wants a database. Todoist wants a project and a due date. They all assume you already know what the thing is. But the moment something matters enough to write down is the moment you know the least about it.

The pain isn't that founders need a better task manager. They have one. It's plain text. The pain is that plain text doesn't carry context, and it doesn't do work. You write \"follow up with Tim\" and that's where it ends. You're still the runtime.

---

#### What a context aggregator is

A meeting notetaker captures one room. Your calendar captures one kind of event. Your inbox captures one channel. Your screen captures what you did. Your notes capture what you thought.

Nothing pulls them together.

Char does. It listens to your meetings. It watches what you do on your computer. It reads your calendar, your email, your Linear, your Slack, your GitHub. And it puts all of it inside one surface — your daily note — where you can also write, on the same line, in the same place. The capture cost stays at zero. The context stops being scattered.

That's the aggregator part. The co-working part is what happens next.

When the context is in one place, a checkbox stops being a string of text. It becomes a job. You write \"follow up with Tim\" and Char already knows who Tim is, what you talked about last week, what he asked for, and what's still open. It can draft the email. It can pull the artifact he wanted. It can put the next step in your daily note tomorrow.

You stay in command. Char moves the work.

The reason this has to be a notepad and not a workspace is the same reason founders use Apple Notes. Workspaces enforce structure before they reward you. Notepads reward you for showing up. If we ask people to learn a new system before Char is useful, we lose them on day one. If we let them type the way they already type and add the context layer underneath, we earn the second day.

---

#### Why the form factor is the moat

I've watched fifteen well-funded teams ship the same product. They take ChatGPT's workspace UI, put a chat box next to a canvas, call it \"AI for work,\" and ship. Codex looks like that. Claude Cowork looks like that. Most of the new YC batch looks like that.

A workspace is a place you go to. A notepad is a place you already are.

The workspace UI fights for your attention. It says: stop what you were doing, come over here, start a new session, give me a prompt. It treats AI as a tool you visit. That's the wrong direction. The future of AI work isn't a place. It's a layer.

Apple Notes won because it stopped trying to be a notes app and became a place to put things. The thing on top of Apple Notes that does the work — that's what nobody has built yet. That's Char.

The form factor isn't a design choice. It's the only place a context aggregator can live without asking the user to change their behavior. Every other product asks. We don't.

---

#### How we charge for it

We locked the business model in May. There are two tiers and one knob.

**Free** is a local-first notepad with on-device meeting capture and bring-your-own-key for any AI feature. It works without a credit card and without us. If you want to use Char as a private notebook with no cloud, you can.

**Pro** is $25 per seat per month, $250 per seat per year. It includes everything cloud — hosted AI, the meeting bot, sync, integrations, screen and workspace context, the team workspace once you add a second seat. It also includes 100 *delegation credits* per seat per month. A delegation credit is one agent action — one email drafted, one report pulled, one calendar slot booked. If you need more, you buy more, at $0.25 to $0.50 per action depending on volume.

We chose to price in actions and not tokens because tokens are not a unit a human can reason about. Cursor priced in tokens last year and watched a quarter of their power users churn the same week the bill arrived. Nobody knows what a million tokens is. Everybody knows what an email is.

Enterprise exists at $50 per seat per month with a sales floor, but we kept it off the public pricing table. We're not selling enterprise yet. We're selling to founders who pay for their own seat.

The pricing reads simple because it is. One seat fee, one usage knob. Everything else is on or off.

---

#### Where we are right now

The Char 1.1.0 closed alpha was supposed to ship the last week of May. It slipped. I'm holding the bar on three things and we don't have all three yet:

1. An editor that feels as good as Philo.
2. A todo list a founder would actually use.
3. Meeting capture that lives inside the daily note, not in a separate tab.

Each of these works in isolation. The interaction between them is what's still rough. I'd rather hold for two more weeks than ship something we'd have to apologize for. We've apologized for shipped things before.

The waitlist sits at **120 signups** with no paid acquisition. Closed alpha runs three sprints. The public launch video lands the last week of June. Public beta in August. We may compress if the product is ready. We won't compress if it isn't.

In parallel, [Anarlog](https://anarlog.so) — the open-source meeting notepad we split out in April — passed **8,500 stars**. We're collapsing its pricing to a single $8 per month Pro tier in early July. Repo stays public, MIT-licensed. We keep shipping fixes at a maintenance cadence. At a 79% margin and roughly $2,500 a month in gross profit, Anarlog covers its own server costs and then some. It is its own product, with its own audience — people who want a clean local-first meeting notepad and nothing else. There is no operational dependency between Anarlog and Char. Two products, two clear stories.

---

#### What I want this to become

The daily note is the wedge. The aggregator is the product. The endgame is something I haven't earned the right to talk about yet, but I'll say it anyway because it's what keeps me building.

Every team I know runs on a graveyard of artifacts. Meeting notes nobody re-reads. Slack threads nobody can find. Linear tickets nobody updates. A wiki that was true in February. Most companies are running on the *idea* of memory. The actual memory lives in two or three people's heads and dies when they leave.

A context aggregator solves the founder's problem first. But every founder I've shown this to has independently said the same thing: I want this for my team. Not as a shared workspace — we have ten of those. As a layer that watches the work and remembers it, so the company has a brain that isn't dependent on anyone's calendar.

I'm not going to ship that this year. I'm going to ship the founder version and earn the right to ship the team version by getting the first one right.

You can write a daily note in Obsidian. You can build a task list in Apple Notes. You can pay for a meeting notetaker, a transcript search tool, a project tracker, an inbox triager. You can chain them with Claude. People do. Half of my customer interviews this month were with founders who had built their own version of this with three tools and a shell script.

It works once. It doesn't compound.

Char compounds because the context is in one place from the start. Tuesday knows what Monday said. The agent that drafts your email at 3pm has read what someone wrote in your meeting at 10am. The checkbox you wrote on your phone last Friday picks up the thread of the spec you wrote on your laptop the week before.

That's the bet. The aggregator is the moat. The notepad is the form.

We'll know in three months whether I'm right.

---

If any of this lands — or doesn't — reply to the update I sent today, or call me at (669) 329-9320. I read every reply.
