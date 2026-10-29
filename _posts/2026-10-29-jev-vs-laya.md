---
layout: post
lang: en
ref: jev-vs-laya
title: "jev or laya: choosing a decision model for your company"
description: Two AI models that only pick from the answers you allow. Which one wins depends on what your company has written down.
permalink: /en/posts/jev-vs-laya/
---

In September 2026 TypeSafe AI launched **Jev**. Three days later Convai released **Laya**, free and open source. The channel Under the Hood AI compared the two in [a short video](https://www.youtube.com/shorts/4Q_YSgS2zMQ). This post sums up what the video shows, and what people running companies should take from it.

## what a decision model is

Jev and Laya are not chatbots. They never write a sentence. You give them a piece of text, such as an email, with the answers you will accept ("scam" or "safe", a score from 1 to 5, yes or no). The model returns a probability for each answer, and nothing else.

Models like this make the small, fast decisions an app repeats thousands of times: routing an email to the right team, blocking unsafe content, helping an AI agent choose its next step.

## a black box and a glass box

- **Jev is a black box.** TypeSafe has not published how it works. You call it over an API and pay per use.
- **Laya is a glass box.** Weights, code and model card are public under Apache 2.0. It is built on ModernBERT, weighs under 1 GB and runs on a laptop.

## the numbers in the video

| | Laya | Jev |
| --- | --- | --- |
| Speed | about 40 ms, on your own machine | about 240 ms, over the internet |
| Cost | free, data stays on your machine | per token, in TypeSafe's cloud |
| Out of the box | 36.2% | 72.7% |
| After training on 1,200 labelled examples | 76.6% | |
| With 77 answers to choose from | about half of Jev | |

The video adds two caveats. The speed race is not fair, because Jev's time includes the trip over the network. And the 1,200 examples used to train Laya came from the same benchmark used to score it.

The most telling detail: given text in Khmer, a script it cannot read, Laya got all 100 wrong while saying it was 95% sure.

## what leaders should take from it

**1. The winner is whoever has labelled data.** Laya only beats Jev once it is trained on labelled examples. Those labels are company knowledge: which team an email belongs to, whether a request is a complaint or a price enquiry. A company that has written those decisions down gets a cheaper, faster option that keeps data in house. One that has not pays for the black box.

**2. "Can't hallucinate" does not mean right.** Both companies make that claim. The model cannot invent an answer outside your list, but it can still pick the wrong one, and pick it with confidence.

**3. Test on your own data before trusting anyone's numbers.** A model that scores 77% on the test it trained for may not hold that level on your company's email.

**4. Privacy is a real reason.** For customer data or contracts, a model that runs on your own infrastructure can matter more than a few points of accuracy.

## which one

Following the video's advice:

- **Jev** when you have no labelled data yet and many answers to choose from.
- **Laya** when you have labelled data, need speed or privacy, and have fewer than 20 answers.

The video's closing line sums up the difference: Jev sells you the answer, Laya hands you the machine. The machine only runs well if you have something to feed it.

*Source: [Jev vs Laya Explained: TypeSafe AI vs the Open-Source Rival](https://www.youtube.com/shorts/4Q_YSgS2zMQ), Under the Hood AI, 25 September 2026. The figures are the video's; VietnamDX has not checked them independently.*
