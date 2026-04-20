---
description: >-
  This is how we build. This guide will set foundational guidelines for every
  engineering project operated by Algorithm.
---

# Engineering Standards

### The Problem We're Solving

When every client works differently, engineering can end up shifting too much toward individual preferences. That might be fine in traditional services, but in an AI-first setup it leads to inconsistency and slows execution over time.

At Algorithm, we follow a strong set of internal engineering guidelines across everything we do. We can adapt to client processes where they're solid, but our baseline standards always stay the same, so quality and speed don't depend on who we're working with.

***

#### 1. AI-Augmented Development as the Baseline

AI tooling isn't a nice-to-have or optional. It's the default standard - just like using version control.

At Algorithm, the approach is intentional:

* Engineers focus on architecture, key technical decisions, and engineering judgment
* They take ownership of system design and the core thinking
* AI handles the repetitive work - boilerplate, scaffolding, first drafts, test generation, and other routine layers

The expectation is that every engineer builds their own AI-enabled workflow where AI is used end-to-end and not bolted on at the end. From initial prompt to final review, AI stays in the loop. Workflows like Claude Code hooks, automated context injection, and AI-assisted PR reviews are things engineers actively build, refine, and share within the team.

Setting up project rules, defining reusable skills, and shaping how AI behaves inside a codebase are all considered good-to-have practices that help teams scale consistency and quality.

At Algorithm, the core tools are Claude Code, Codex, and Cursor. Every engineer actively uses them, is comfortable with them, and continuously improves how they work with them — not just aware of them.

***

#### 2. Design Docs for Every Major Decision

Before any significant feature gets built or any major technical decision gets made, a design doc is written.

A design doc at Algorithm has:

* At minimum three solution approaches to the problem
* A clearly recommended solution with reasoning behind it
* Sign-off from the tech lead on the project before work begins
* The document should be hosted in a shared google drive for the specific project

If the project has no tech lead available, the design doc gets reviewed by a senior engineer from outside the project. The point is that no significant decision ships without a second technical mind having looked at the approach first.

This is the gate between thinking and building. Skipping it is how teams build the wrong thing cleanly.

***

#### 3. PR Culture with a Hard Standard

Every line of code that hits main goes through a pull request. Branch protection is on and the PR is the only path to production.

A PR at Algorithm has:

* A clear description of what changed and why
* A self-review checklist (AI generates it, the engineer owns it)
* At least one reviewer before merge
* A 48-hour rule — anything sitting without a review gets a comment or an escalation
* Connect it with its associated issue/ticket to self close the issue/ticket when PR is merged

On ownership of reviews:

* The tech lead on the project is the primary reviewer and the one approving significant changes
* Any peer engineer can review and merge code once they've built the trust on the project — this is earned, not assumed

Quality is defined at the PR level — where code is actually written, reviewed, and merged.

***

#### 4. CI/CD Ownership, Not Just Setup

Having CI/CD is the starting point. Owning it is the standard.

* Every new project ships with a CI/CD pipeline from a suitable point of time
* Every engineer on a project understands the pipeline — not just the tech lead
* The pipeline is accountability made visible, not just infrastructure

On breakage:

* The engineer who breaks CI fixes CI and owns end to end
* Responsibility stays with the person who introduced the change, not whoever's available

If something breaks and no one knows why, that's a knowledge silo. Silos are a liability here.

***

#### 5. Documentation as a Deliverable

Documentation is part of the sprint — not a task saved for after delivery.

Every feature, every architectural decision, every non-obvious implementation — documented. Enough that someone new can get running locally within an hour.

The rule:

* If a project is missing that foundational README, the first engineer who onboards onto it writes it
* That is their first contribution
* The documentation written today is the onboarding cost not paid later

This is what makes Algorithm scalable — not just headcount.

***

#### 6. Retrospectives That Actually Surface Truth

One retro per sprint, per team. The format is flexible. The outcome is not.

What we're looking for:

* "This process slowed us down"
* "I didn't understand the requirements before I built it"
* Systemic signals — not individual blame

The only hard rule: one concrete process improvement comes out of every retro — even a small one. A retro that ends with no action item was a meeting, not a retro.

***

#### What We Preach

**Ship with intent.** Fast delivery is a value. Shipping fast without knowing why the feature exists is noise. Every engineer understands the user problem before they open their editor.

**AI is a multiplier, not a substitute.** The right setup lets you reach further than you could alone. It doesn't replace judgment — it frees up more time to use it. An engineer using AI to avoid thinking will be obvious very quickly.

**The PR is your signature.** A vague description or an unexplained decision stays in the codebase long after the sprint closes. Own what you put out.

**Silos are a liability, not job security.** If you're the only person who understands how something works, you've created a risk — not a safety net. Document it, pair on it, hand it off.

**We don't celebrate firefighting.** When something breaks and someone saves the day, the first question isn't "great job" — it's "why did this happen?" Heroics are a symptom. A tight process is the goal.

***

#### Three Things to Do Now

* **Write the internal doc.** Two pages max — _How We Build at Algorithm._ Non-negotiables only. Every engineer reads it and acknowledges it. Revisit it quarterly.
* **Audit CI/CD coverage.** Which projects have it, which don't. The ones that don't get a two-week deadline. Tech lead owns that.
* **Name an Engineering Standards owner.** One of the best engineers — not the tech lead whose plate is full. Their mandate: flag when teams drift from the standard, propose improvements, own the internal bar.

***

#### The Vision

Algorithm engineers ship production-grade software faster than most in-house teams — not because they grind harder, but because the process is tighter and AI is in every layer of how they build.

Architecture and high-level decisions come from us. Everything beneath that — the implementation, the tests, the scaffolding, the repetitive layers — gets built with AI at the core, from the first prompt to the final review. Engineers here don't just use AI tools. They build development systems around them. Claude Code, Codex, and Cursor are the starting point. What each engineer builds on top of that is what separates good from great.

PRs are where quality gets enforced. Design docs are where bad decisions get caught before they become bad code. Pipelines run on every project. New engineers onboard from a README. When something breaks, the person responsible fixes it.

The standard is internal. Clients see the output. The culture is ours.
