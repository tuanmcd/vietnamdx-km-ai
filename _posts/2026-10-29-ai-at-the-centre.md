---
layout: post
date: 2026-10-29 14:00:00 +0700
lang: en
ref: ai-at-the-centre
title: "put AI at the centre: lessons from the head of claude code"
description: Anthropic raised code output per engineer eightfold by putting AI in the middle of every process and clearing one bottleneck at a time. What leaders can take from it.
permalink: /en/posts/ai-at-the-centre/
---

In a conversation with Mark, the host on AMD's side, Boris, who created and leads Claude Code at Anthropic, describes how his company works now that AI sits inside every process. This post sums up the [34-minute video](https://www.youtube.com/watch?v=c4kYurm0hD8) and picks out what matters to people running companies.

## the computer in the corner

Boris recalls a Harvard Business Review article from the 1990s that asked why computers had not raised productivity. Its answer was that there were two kinds of company:

- **The first** put a computer in a corner of the office and kept the paper, pens and filing cabinets. Productivity stayed flat.
- **The second** threw out the filing cabinets and put the computer at the centre of every process. Those were the companies that saw real gains.

AI is the same, Boris says. The most successful adopters of Claude put it at the centre, not off to the side.

## new hires ask the AI, not the wiki

His example is a first day at Anthropic. At most companies, to find the office address, get access to the code base or file an expense report, you search a wiki or ask a colleague. At Anthropic you ask Claude.

From there Claude stays in everything: writing code, reviewing it, checking security, gathering user feedback, triaging incidents, brainstorming products. Not only in engineering, but in product, design, marketing and sales.

What Boris leaves unsaid, and leaders should notice: Claude can answer a new hire only because those answers **were written down somewhere**. Putting AI at the centre means putting the organisation's knowledge at the centre. Today's version of throwing out the filing cabinet is moving processes, policies and experience out of inboxes and heads and into a place the AI can read.

## one bottleneck at a time

Since the start of the year, code output per engineer at Anthropic has risen eightfold. Large customers, Boris says, are seeing 50 to 150%, against the few percent a year a company usually manages.

The method is plain: find the biggest bottleneck, give it to the AI, then find the next one. First coding. Once code is faster, review becomes the bottleneck, so that goes to the AI too. Then sales material. And so on.

Once engineering stops being the bottleneck, the bottleneck becomes **how fast you can come up with good ideas and bring them to market safely**.

## from one agent to thousands

Boris describes the stages companies pass through:

| stage | how people work |
| --- | --- |
| 1 | each engineer runs one agent, still one task at a time |
| 2 | about 10 agents, switching between sessions |
| 3 | dozens to hundreds, agents handing work to sub-agents |
| 4 | thousands, the AI coordinating whole teams on big jobs |

Most companies, in his view, sit between stages 1 and 2; Anthropic averages stage 3. His stage-4 example: Stripe moved a body of Scala code to Java in four days instead of months.

## ROI: don't only look at the I

This is the part most worth a leader's time. Many companies measure AI's ROI by cutting cost: cheaper models, lower reasoning effort. Boris says you should do that, but **the R matters more**: the return.

Raising the R means letting people experiment. The best idea often comes not from your most senior engineer but from a new graduate, or a marketer somewhere in the organisation. Once a use proves itself, then you optimise its cost. Skip the experimenting and you never find the opportunity.

Mark adds an example from AMD: a chip bug that a team had failed to solve for weeks, which a junior engineer cracked using agents. That did more to convince senior engineers than any presentation.

## the leader's job

Boris sums up his own role in two parts:

1. **Make it safe to try.** Nobody gets a poor review for trying a new idea. If leaders don't make room, people keep working the old way.
2. **Give people context.** Business context, product context, so they can make better decisions on their own.

The second applies to the AI as well. As models improve, Boris says, he works with one like a senior engineer: trust it, give it context and goals, check in. That context has to live somewhere before it can be handed over, to people or to machines.

## how to measure, and how far to trust

- **Evals and vibes.** For a workflow repeated thousands of times, you need evals to know whether a new model is better. For other things, people's judgement goes a long way, because evals cost effort to write.
- **Stop the endless "yes".** When an agent asks for approval too often, people stop reading and just press yes. Anthropic moved approval to an automatic classifier, tested through evals and penetration testing, and found it safer.

## the next six months

Boris won't predict two or three years, only six months: agents running longer, each person running more of them, less course correction. Running agents for days at a time will become normal, and whole products, even startups, built by Claude may start to appear.

## three questions for your next leadership meeting

- Is our AI in the corner or in the middle of our processes?
- When a new hire asks it something, does it have the right answer, and where does that answer come from?
- Are we measuring AI by the cost it cuts, or by the new things it lets us do?

*Source: interview with Boris (Anthropic) on AMD's show, reposted by the channel hyperfixation on AI as [Stop Prompting — Head of Claude Code Uses Opus 5.5 + Graphs + Harness](https://www.youtube.com/watch?v=c4kYurm0hD8), 22 October 2026. Note: the repost's title and description mention graphs, harnesses and memory, but the conversation does not cover them. Figures are the interviewee's; VietnamDX has not checked them independently.*
