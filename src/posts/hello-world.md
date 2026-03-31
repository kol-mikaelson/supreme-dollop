---
title: "On building things that last"
date: 2026-03-31
description: "A note on why I care more about the substrate than the surface, and what that means for how I write software."
tags: [engineering, craft]
layout: post.njk
---

There's a kind of software that feels like it was built to be replaced. You can tell when you're reading it — the abstractions are thin, the decisions are deferred, the tests are aspirational. It works, in the sense that it ships. But it doesn't *hold*.

I've been thinking about what separates that from software that lasts.

## The substrate matters more than the surface

Most discussions about software quality focus on the visible layer — the API design, the UI, the performance numbers. These things matter. But they're downstream of something more fundamental: the quality of the substrate. The data model. The error handling philosophy. The naming conventions. The choices that nobody sees but that every future decision inherits.

When the substrate is wrong, everything built on it is fighting an uphill battle. Features that should take hours take days. Bug fixes introduce new bugs. The system resists change because it was never designed to accommodate it.

When the substrate is right, the opposite happens. The codebase becomes *generative*. New features fall naturally out of existing abstractions. The system rewards understanding.

## Boring decisions are load-bearing

One of the things I've learned is that the least glamorous decisions are often the most important.

Should error handling be done with exceptions or explicit return types? Should this be one table or two? Should this abstraction be a class or a function? These questions don't make it into architecture documents. They're made quickly, in the middle of other work, under pressure. But they compound. Five years later, they're the reason a migration is possible or impossible.

I've started treating these small decisions with the same care I'd give a larger one. Not because every decision deserves a committee — the opposite. Because the discipline of asking "what am I actually optimising for here?" before making a choice is fast, cheap, and catches a surprising number of mistakes.

## On the patience required

Building things that last requires a particular kind of patience that is slightly out of fashion. The pressure to ship fast is real. The desire to be done is real. The temptation to defer the hard question to a future version of yourself is very real.

But I've found that the best engineers I've worked with share a willingness to sit with discomfort longer than average. To say "I don't have a good model for this yet" and actually mean it as a reason to pause, not just a disclaimer before proceeding anyway.

That patience isn't slowness. It's the difference between taking ten hours to build something that lasts and taking eight hours to build something you'll spend the next year fighting.

---

These are just notes. I'll keep writing as I figure this out.
