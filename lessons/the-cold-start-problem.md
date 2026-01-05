---
title: "The Cold Start Problem"
author: "Andrew Chen"
created_at: "2023-04-21 11:30:12.798127+00"
description: "Learning notes on Andrew Chen's network effects and solving the cold start problem."
---

Before diving in, this is a book I keep coming back to whenever I have concerns about business. Even after reading it multiple times, it doesn't become clear what I should do, but I read it because it seems to give me new insights each time.
Link: [The Cold Start Problem by Andrew Chen](https://www.coldstart.com/)

# Network Effects

## What's a Network Effect, Anyway?

> In its classic usage, **a network effect describes what happens when products get more valuable as more people use them**.

There are networks where network effects strengthen as more people join, but there are also cases like IoT where network effects strengthen as more sensors are added. In this way, "having network effects" means **the more nodes that make up the network, the stronger the network's power becomes**.

> A telephone without a connection at the other end of the line is not even a toy or a scientific instrument. **It is one of the most useless things in the world**.

by Theodore Vail, former President of AT&T

Whisper is the same. From a writer's perspective, if there's no one to read, they won't feel any value. The difference is that since it's asynchronous communication, you just need to create that feeling. For this, you enable various interactions like likes, comments, replies, and following.

> The "network" is defined by **people who use the product to interact with each other**. For AT&T's telephone network, it literally consisted of the wiring that spanned between homes.

> The "effect" part of the network effect describes **how value increases as more people start using the product**. Sometimes the increasing value manifests as higher engagement, or faster growth. But another way is to think about it as a contrast---at its beginning. YouTube didn't have any videos, and neither viewers nor creators would find it valuable. But today, YouTube has nearly 2 billion active users watching a billion minutes of video per day, and this in turn creates engagement between creators and viewers, viewers and each other, and so on.

How should the network's value increase in Whisper? For each user making up the network to feel the value of that network, shouldn't they be able to track their posts and comments?

> ... how do you tell if a product has a network effect, and, if yes, how strong is it? The questions to ask are simple: First, **does the product have a network?** ... And second, **does the ability to attract new users, or to become stickier, or to monetize, become even stronger as its networks grows larger?**

Does Whisper have a network? Yes.

Does Whisper become stickier as users increase? I'm not sure. From a producer's perspective, more users means more audience they can reach, which is good. But if there's no way to know this, and if metrics can't be gathered and checked in one place, it's all pointless. In this regard, the stickiness consumers feel depends on producers. If content isn't produced, all consumers will leave.

> ... it's not a great time to launch a new product. ... competition is fierce, copycats abound, and marketing channels are ineffective.

> We are now in a zero-sum era of attention with minimal defensibility for a vast swath of mobile app, software-as-a-service (SaaS) products, and web platforms.

> No wonder the top app charts now rarely change, and are mostly dominated by large, established products.

> While Instagram might be able to copy Snapchat's features like Stories or ephemeral photo messages in a few months, **it's difficult to change the behavior of millions of consumers to switch over**.

Similarly, you can copy features from Everytime or Twitter, but it's hard to drive behavior change in the customers they already have.

> **Knowledge workers increasingly have the same "it just works" expectations on enterprise software**, as they do with the apps they use at home. Increasingly, this means the **enterprise is becoming "consumerized" with software that is adopted by individuals**, then spread within the company's network---with network effects.

## Cold Start Theory

> Solving the Cold Start Problem requires getting all the right users and content on the same network at the same time---which is difficult to execute in a launch.

> ... an approach the focuses on building an **"atomic network"**---that is , **the smallest possible network that is stable an can grow on its own**. For example, Zoom's videoconferencing network can work with just two people whereas Airbnb's requires hundreds of active rental listings in a market to become stable. ... **who are the first, most important users to get onto a nascent network, and why? And how do you seed the initial network so that it grows in the way you want?**

# The Cold Start Problem

## Tiny Speck

> First, I start with a principal dilemma, which I call **"Anti-Network Effects"**. It's a myth that network effects are all powerful and positive forces---quite the opposite. **Small, sub-scale networks naturally want to self-destruct**, because when people show up to a product and none of their friends or coworkers are using it, they will naturally leave. What solves this? **"The Atomic Network"**---**the smallest network where there are enough people that everyone will stick around**.

What I felt while using BeReal is that 3 friends besides myself started together and have been using it continuously for 5 months. Of course, I had signed up before to try it out, but I looked around and immediately left. If I had used it with just 1 friend, it wouldn't have meant much more than exchanging photos via KakaoTalk. In that sense, I think BeReal's atomic network size is about 3-4 people.

> These networks often have "sides", whether they are buyers and sellers, or content creators and consumers. ... However, the most important part of any early network is attracting and retaining **"The Hard Side"** of a network---**the small percentage of people that typically end up doing most of the work within the community**.

> To attract the hard side, you need to "Solve a Hard Problem"---**design a product that is sufficiently compelling to the key subset of your network**.

> When the Cold Start Problem is solved, a product is able to consistently create "Magic Moments." Users open the product and find a network that is built out, meaning they can generally find whoever and whatever they're looking for.

## Anti-Network Effects

> The reality is that new products are often greeted by a nice initial spike of users, but this falls to a trickle as the novelty wears off. ... **People won't use their product unless their friends are on it**.

> Slack works with just 2 people, but it takes 3 to make it really work. There are long-running 3 person groups that are stable---that's the minimum required to be called a customer. 

by Stewart Butterfield, CEO of Slack

> Based on our experienc of which companies stuck with us and which didn't, we decided that any **team that has exchanged 2,000 messages in its history has tried Slack---really tried it**." ... "But it hit us that, regardless of any other factor, after 2,000 messages, **93% of those customers are still using Slack today**.

by Stewart Butterfield, CEO of Slack

> For new products, it's important to **have a hypothesis for the size of your network even before you begin**. Communication apps can be 1:1, so the network is small, and you can plan accordingly. Contrast that to products that are highly asymmetrical, with content creators and viewers, or marketplaces with buyers and sellers---these are likely to require a much bigger number to hit the threshold, and require a much bigger effort to get started. The size of an initial network helps determine a launch strategy.

> **You need the right people on the network**. Ten people using Slack all from the same team is better than ten random people in a larger company. **Density and interconnectedness is key**.

Should we also use Whisper as a place for confession among ourselves, and gradually recommend friends to confess there?

## The Atomic Network

> If you study the launch of products with network effects, you'll see that one of the most common threads is that **they often start small**, in a single city, college campus, or in small beta tests at individual companies---like Slack's story.

> The networked product should be launched in its **simplest possible form**---not fully featured---so that is has a **dead simple value proposition**. The target should be on **building a tiny, atomic network**---the smallest that could possibly make sense---and **focus on building density**, ignoring the objection of "market size". And finally, the attitude in executing the launch should be **"do whatever it takes"**---even if it's unscalable or unprofitable--to get momentum, without worrying about how to scale.

> **Disruptive technologies are dismissed as toys because when they are first launched they "undershoot" user needs**. The first telephone could only carry voices a mile or two. ... What they failed to anticipate was how rapidly telephone technology and infrastructure would improve (technology adoption is usually non-linear due to so-called complementary network effects). The same was true of how mainframe companies view the PC (mircocomputer), and how modern telecom companies viewed Skype.

by Chris Dixon, General Partner @ a16z

> Underestimating new products in this way is the number one way to make dumb predictions in the tech industry. It's what leads pundits to say a product won't work, isn't interesting, or has a small market size---followed by that product proving them wrong just a few years later.

> It's not that product changes are needed---it's that **the network needs to fill out to the point where people and content are relevant**.

> The first step to launching an atomic network is to **have a hypothesis about what it might look like**. My advice: Your product's first atomic network is **probably smaller and more specific than you think**. ... It was similar for Uber, whose networks we tend to talk about as "San Francisco" or "New York", but in the earliest days, the **focus was on narrow, ephemeral moments**---more like **"5pm at the Caltrain station at 5th and King St."** The general managers and Driver Operations had an internal tool, called Starcraft---referring to the real-time strategy game popular at the time---that allowed them to click on a group of cars, text them "Go to the train, lots of riders!" and direct them in real time.

> ... because **what's easier for you will be easier for your competitors**---they just need a few users to get started as well, which is why there are so many messaging apps and chat features inside larger products.

> Growing city by city, campus by campus, or team by team is a surprisingly powerful strategy. It leads to dense, organic connections of users that strengthen network effects across multiple dimensions: **Engagement goes up**, because users are **more likely to find other relevant user**. **Viral growth goes up** when prospective users of a product **sees that their friends and colleagues are all using the service**.

## The Hard Side

> ... there is a minority of users that create diproportionate value and as a result, ha...
