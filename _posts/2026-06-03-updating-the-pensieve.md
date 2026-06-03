---
layout: single
title: "Updating the Pensieve with Smoother Note Entry"
description: "A process update on the Pensieve - introducing the Note Generator to reduce the friction of adding research notes."
date: 2026-06-02 21:30:00 -0400
last_modified_at: 2026-06-02 21:30:00 -0400
author_profile: true
comments: false
tags: [research, phd, academic-notes, knowledge-management, semantic-search, AI-in-research, research-tools]
excerpt: "A quick process update on the Pensieve: the Note Generator is a form that makes it simpler to consolidate my research notes, and some deployment improvements under the hood."
---

A quick update on the [Pensieve](https://pensieve-live.streamlit.app/) — a tool I introduced [earlier this year](https://rehanmirza.net/introducing-the-pensieve/) for searching across my research notes and papers.

<!--more-->

One thing that's been slightly clunky about using the Pensieve is adding new notes. This has meant hand-formatting a Word document to a specific heading structure: Heading 2 for subtopics, Heading 3 for each paper, URL and author lines in the right places. The indexer is picky, and getting it wrong meant things didn't surface in search. Having to go into documents also meant this was a process I deferred to the end of the past two semesters, creating a tedious process to copy over and reformat all my readings in one go. 

I've added a small local web form – the **Note Generator** – to smooth this out. First, open up 'taxonomy.csv' to define your research areas (i.e., 'buckets') and associated subtopics:

![Defining research areas and subtopics](/images/posts/pensieve_update/Taxonomy_CSV.jpg)

Then open up the 'Note Generator.bat' file, providing admin access as needed. Choose the bucket (in my case corresponding to my eight research areas) and subtopic, then the semester:

![Form overview – bucket, subtopic and semester selection](/images/posts/pensieve_update/Form_overview_1.jpg)

Then fill in the paper details:

![Form overview – paper metadata fields](/images/posts/pensieve_update/Form_overview_2.jpg)

And your notes by section (sections are customisable):

![Form overview – notes by section](/images/posts/pensieve_update/Form_overview_3.jpg)

Hit save and a correctly-formatted `.docx` lands in the right folder, ready for the indexing pipeline to pick up. Both form-generated and hand-written docs continue to work side by side.

I also tidied up the deployment pipeline, making it more robust for regular updates.

## Try it yourself

The full project is available on [GitHub](https://github.com/ramirza1/pensieve-project-template) – including the Note Generator. The README has setup instructions.

## A note on AI

As I outlined in my [first post on this tool](https://rehanmirza.net/introducing-the-pensieve/), I used AI to help build the Pensieve, and it relies on AI in operation for embeddings and summaries. I'm continuing to think carefully about where and how I use it – conscious of the real concerns around skills atrophy, labour exploitation, and over-reliance. I also note its promise to support better research, hopefully for social good.