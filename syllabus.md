---
layout: page
title: Syllabus
permalink: /syllabus/
---

**M.Eng. Project: The Invisible Work Initiative**

Can AI recognize, perform, and model the work that keeps software alive?

**Project Advisor:** John Meluso, PhD

## About this Project

**Project Advisor** John Meluso, Systems Engineering Program, Cornell University.

**Project Area** Open Source Ecosystems, Human-AI Collaboration, AI Agents, Benchmarking and Evaluation, Data Science, Agent-Based Modeling, Sociotechnical System Design.

**Project Keywords** Artificial Intelligence; Invisible Labor; Open Source Sustainability; AI Agents; Benchmarks; Agent-Based Modeling; Human-AI Teaming; Triage.

### How do I join?

To apply, [fill out the project application here](https://forms.gle/x56KEJ5Pex9PAeTU9). You'll be asked to include a resume/CV and some information about yourself! I encourage you to answer in your own words so I can get to know you; don't worry, I don't expect perfect spelling or grammar.

If you receive an invitation to join:

- **Systems Engineering Program.** Complete and submit the SYSEN project form to the program office. Register in the appropriate SYSEN 5900 section (section number to be confirmed before the semester starts).

- **Another Program.** Complete and send me your program's form to sign. Register in an appropriate project section as instructed by your program. Please investigate what your program expects and share what you learn with me. We'll finish the process together.

## Project Description

Software of all kinds depends on work that few people see. Reviewing bug reports, judging their severity, detecting duplicates, mentoring newcomers, and deciding what a confusing request is really asking for are all examples of this. Tasks like these keep critical software operating, but they rarely leave the kind of visible record that code does. This is called [invisible work](https://dl.acm.org/doi/10.1145/3757417).

For years, open source workers (in software and other fields) have been straining under invisible workloads. Rather than fixing things, AI is generally making things worse, often much worse. For instance:

- [Census III](https://www.linuxfoundation.org/press/open-source-usage-trends-and-security-challenges-revealed-in-new-study), by the Linux Foundation and Harvard, found that 40 percent of the most widely used open source projects depend on one or two developers for more than 80 percent of contributions. This makes them vulnerable to attacks and growth of AI submissions.

- In November 2025, [Kubernetes retired Ingress NGINX](https://www.kubernetes.io/blog/2026/01/29/ingress-nginx-statement/), a component used in roughly half of cloud computing environments. Development had fallen to one or two people working in their spare time; no replacements could be found.

- In January 2026, curl, a widely-used data transfer program, [ended its bug bounty program](https://www.theregister.com/2026/01/21/curl_ends_bug_bounty/) due to an influx of AI-generated vulnerability reports. curl's small volunteer security team couldn't keep up. Django, Node.js, and libxml2 restricted their intake processes for the same reason.

- Meanwhile, benchmarks for AI coding agents, such as the [SWE-bench](https://arxiv.org/abs/2310.06770) family, measure whether an agent can produce a code patch that resolves an issue. None of them measure the judgment work described above.

The thesis of this project:

***AI systems produce vast amounts of visible work. But small numbers of humans perform the invisible work of judging and coordinating work with stakeholders. Humans alone cannot keep up with AI products. This asymmetry is breaking organizations and computing infrastructure.***

This project builds one system that addresses part of this problem: an automated quality checker for incoming bug reports. Several teams build the system together. Each team owns one part and depends on the others' work (see Project Teams below).

**How I run projects.** I will give you a goal, targets, and kind, honest feedback. I will not give you a recipe. This means your team gets to make the decisions, write down your reasons, and ask for help when stuck. Yes, you're likely to make lots of mistakes, which is great! ***Mistakes are how we learn.*** I expect us all to create an environment where everyone feels safe to make mistakes. So you'll experiment, try things, fail sometimes, and try again. An important rule, though: If a problem has blocked you for more than three days, you must take it somewhere (a teammate, another team, a public forum, an AI assistant). Staying silently stuck is the one form of failure this course does not credit. So help each other and we'll make progress as a team!

## Project Teams

This project builds one system: an automated quality checker for incoming bug reports. The teams below build it together. Each team owns one part of the system and depends on the others' work.

**Software Systems Engineering Team.** This team decides what the system must do and how we will know it works. You will write the requirements, design the shared format for findings, and define the interfaces the other teams build to. You will assemble a dataset of historical bug reports from several open source projects, build the baselines, and build the evaluation that measures every part of the system. You will also own how reports enter the system and how findings are returned to the maintainer. You can show employers that you can lead requirements, verification and validation, and integration on a real system.

**Report Analysis Team.** This team judges a report on what it contains. You will decide whether a report includes what a good bug report needs, such as steps to reproduce and a clear statement of expected versus observed behavior. You will turn published research on bug report quality into checks the system can run. Each check produces a finding the maintainer can inspect. You can show employers that you can turn a research literature into a working evaluation of text.

**Claim Verification Team.** This team checks whether a report's claims are true. You will find the files, functions, and commits a report cites and confirm that they exist and behave as the report says. The lowest-quality reports often cite code that is not there, so this work matters. You will work directly against real codebases and their version history. You can show employers that you can analyze code and detect unsupported claims.

<!-- FOUR-TEAM VERSION. To use four teams instead of three, delete the three team descriptions above (keep the heading and intro paragraph) and uncomment the block below.

**Software Systems Engineering Team.** This team decides what the system must do and how we will know it works. You will write the requirements, design the shared format for findings, and define the interfaces every other team builds to. You will assemble a dataset of historical bug reports from several open source projects, build the baselines, and build the evaluation that measures the whole system. You can show employers that you can lead requirements and verification and validation on a real system.

**Integration Team.** This team builds the layer that connects the other teams' work. You will take an incoming report, pass it to the analysis teams, collect their findings, and assemble the single report the maintainer sees. You will state clearly what the system could not check. As a stretch, you may connect the system to GitHub so that a new issue is reviewed automatically. You can show employers that you can design and build the integration layer that turns separate parts into one working system.

**Report Analysis Team.** This team judges a report on what it contains. You will decide whether a report includes what a good bug report needs, such as steps to reproduce and a clear statement of expected versus observed behavior. You will turn published research on bug report quality into checks the system can run. Each check produces a finding the maintainer can inspect. You can show employers that you can turn a research literature into a working evaluation of text.

**Claim Verification Team.** This team checks whether a report's claims are true. You will find the files, functions, and commits a report cites and confirm that they exist and behave as the report says. The lowest-quality reports often cite code that is not there, so this work matters. You will work directly against real codebases and their version history. You can show employers that you can analyze code and detect unsupported claims.

-->

## Who Should Apply

You should apply if you're interested in practicing the following:

- **Decision-making amidst ambiguity.** Working on unsolved problems (like this) creates opportunities for you to practice making decisions amidst ambiguity. Sometimes we will not know the right answer, or there will not be a right answer at all. You don't need to be comfortable with ambiguity—most people aren't, including me! But practicing making decisions with supporting evidence on a project like this will make it easier, though.

- **Workplace Application of AI Models.** Whether you love AI or hate AI, you will learn what the frontier AI models can and cannot do in organizational contexts, even as capabilities evolve. What workplace activities do AIs do well, and where do they fall short? How can we bridge the gap? This is evolving, and you'll help us figure all of this out.

- **Teamwork.** The best companies *only* hire people who work well in teams. This project will help you prove that you can do this. You'll practice teamwork by giving each other regular (kind) feedback, carefully deciding interface requirements together, communicating about deliverables, and holding each other accountable.

Python is our working language. Prior experience with AI systems, security, simulation, or open source is useful but not required. Willingness to learn in public is required.

## Attendance

- One all-hands meeting every two weeks (about an hour) where each team shares progress, decisions, and blockers. Gate rehearsals happen here.

- One weekly team check-in with me, scheduled per team in the first week of class. In these meetings, I don't need you to prove to me that you're making progress – that's what the gates are for. Instead, these are for you. What do you need? What questions do you have? What do you want feedback on? Just come prepared with something to discuss that helps your team advance toward its goal.

## Grading Criteria

Each semester, you will earn credit for successful gate reviews, peer evaluations, and a self-assessment. An ambitious attempt that partially fails, with a clear account of what you learned, is worth more than a safe attempt that fully succeeds.

- **50% Gate Reviews (by team).** Two stage gate reviews, weighted 20% and 30% respectively. You will present what you decided and why, what you learned and built, and what you tried and abandoned. Failure and success can both earn credit as long as your team provides evidence.

- **30% Peer Evaluations.** Members of the other teams will evaluate what your team produced. Other members of your team will evaluate what you produced.

- **20% Self Assessment.** What you contributed, what you did well, what you did not do as well as you wanted, what you would do differently, what you can do in your next role.

## How we Work Together

All project work is developed in the [Invisible Work Initiative's repositories](https://github.com/invisible-work-initiative) under open licenses. Joining the project means you agree to work this way. Our primary language is Python, but we'll use other languages as needed. Code will be fully reproducible. All work goes into public repositories under open licenses from the start, not at the end. You will experience both the benefits and the frictions of working in the open. Each gate deliverable must be reproducible by a teammate from the repository alone. If it only runs on your laptop, it does not exist. AI tools are permitted and expected. You are accountable for everything you submit. Submitting unverified generated work that others must review is the exact failure this initiative exists to address.
