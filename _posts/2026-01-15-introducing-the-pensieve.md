---
layout: single
title: "Introducing the Pensieve"
description: "A tool to help me retrieve important knowledge from an ever-expanding set of research notes - and one I'm sharing with the research community."
date: 2026-01-15 22:00:00 -0500
last_modified_at: 2026-01-15 22:00:00 -0500
author_profile: true
comments: false
tags: [research, phd, academic-notes, literature-review, knowledge-management, semantic-search, AI-in-research, research-tools]
excerpt: "I built the Pensieve: a search tool that helps me trace concepts, authors, and arguments across my ever-expanding set of notes and papers."
---

As I go through my PhD, my notes are going to expand evermore. To keep track, I've designed a searchable repository to help me track and trace concepts across the years. I'm sharing this tool [(an ongoing work in progress!)](https://github.com/ramirza1/pensieve-project-template) with the research community, in the hope it will be useful to others.

<!--more-->

## Novels of notes

In preparation for my PhD applications and through my first semester, I read 117 papers. My notes total ~90,000 words. To fully go through and digest them, I have to read the equivalent of a book. A rambly, incohesive book largely in the form of bullets and riddled with typos. That's somewhere between the length of "Harry Potter and the Chamber of Secrets" and "Harry Potter and the Prisoner of Azkaban". However, I'm probably not being published by Penguin anytime soon.

Nevertheless, I am going to have to digest and thread through those notes, which will probably have grown into an unholy trilogy by the time I write my comprehensive exams next year. By then, my readings on discourse quality measurements, top of mind for so much of last semester, may be reduced to "fingerprints on an abandoned handrail", to borrow a wonderful turn of phrase from Bob Mortimer (incidentally I'm currently on a *Would I Lie to You* kick as I wait for my code to run: [link](https://www.youtube.com/watch?v=MsuuiVzS6Js)).

## A search engine for my brain

To address this, I built the Pensieve. This is effectively a search engine for my notes. I can track down which sections most closely relate to concepts, authors or other potential search terms of interest. I can also read brief summaries of each paper, and generate an excerpt of its relevance to the search term of interest. At the same time, I know this is bounded to my own work, and grounded in my own interpretations of each paper.

## Try it yourself

If you'd like to take a look at how the tool works, you can check out a [live demo of the tool](https://pensieve-live.streamlit.app/). If you'd like to build out your own version of the tool, you can find the [code on GitHub](https://github.com/ramirza1/pensieve-project-template). You can configure the tool to either run locally, or host it on a web server. Please read through the README carefully to figure out how you can organize your notes and set up the tool.

## On the use of AI as a research tool

One elephant in the room to address: the use of generative AI as a research tool. There's legitimate concern around this, and I'm still figuring out and iterating my own approach to the technology. There are real moral concerns and pitfalls. Just this week, I came across a thoughtful passage on AI policy in the syllabus of one of my courses, that pointed out the exploitative nature of the technology for the Global South. I am also conscious of a potential skills atrophy - for instance in using it as a writing aid - and more pertinently, potential skills 'bypass', where for instance I never learn to code because I can muddle through with AI.

At the same time, as was pointed out in another course, AI undoubtedly can increase our capacity to do quality research. So I'll set out my stall - I used AI to build this tool, and it is also reliant on AI in its operation, to generate embeddings for search functionality, and to generate summaries. I will be using AI to enhance the efficiency, reliability, and capacity with which I can do my research, but I will also make sure I'm in full control and knowledge of what I'm doing.

I hope this tool will be useful to other researchers. I'd also love to work with collaborators to see how I could improve it further - particularly on the UI and additional functionality.