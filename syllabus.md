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

This project has three tracks which will explore different aspects of this problem. Can AI recognize invisible work (Track 1)? Can it responsibly perform part of it (Track 2)? What happens to a human-AI collective when it cannot (Track 3)? The tracks share one vocabulary and depend on each other's outputs (see Interfaces below).

**How I run projects.** I will give you a goal, targets, and kind, honest feedback. I will not give you a recipe. This means your team gets to make the decisions, write down your reasons, and ask for help when stuck. Yes, you're likely to make lots of mistakes, which is great! ***Mistakes are how we learn.*** I expect us all to create an environment where everyone feels safe to make mistakes. So you'll experiment, try things, fail sometimes, and try again. An important rule, though: If a problem has blocked you for more than three days, you must take it somewhere (a teammate, another team, a public forum, an AI assistant). Staying silently stuck is the one form of failure this course does not credit. So help each other and we'll make progress as a team!

## Track 1: The Invisible Work Benchmark

**Overview.** Can current AI systems recognize invisible maintainer work at all? Nobody has tested this. You will build the first benchmark that does, from public data. This could include a public benchmark dataset, an evaluation harness, and a findings report measuring how well leading AI models identify invisible maintainer tasks. The initial plan is to start with two relatively simple task types whose correct answers are the most objective: duplicate detection (was this issue later closed as a duplicate, and of what?) and report validity (was this security report later confirmed or rejected?). Both have documented historical outcomes in public data (like past GitHub Issues), which is what makes evaluation possible. Other task types are stretch goals to pursue only after the pipeline works.

**What you'll create.** A calibration study of your own judgment against historical outcomes, a public benchmark dataset, an evaluation harness, and report of findings. Together these demonstrate data engineering, evaluation design, and judgment about AI capabilities: skills employers actively seek.

**Need.** 3 to 5 students. Python experience preferred. Also useful are API experience, basic statistics, and patience for careful labeling. No prior ML evaluation experience required.

## Track 2: The Triage Sentinel

**Overview.** One part of invisible work is so dull, dirty, and dangerous that people are quitting over it: reviewing large quantities of low-quality, often AI-generated reports (called "triaging"). Can an AI system effectively triage incoming reports? You will build the system and provide evidence that it works. This is likely to include an open source tool that pre-processes incoming issues or vulnerability reports for a project, tasks like clustering duplicates, checking claims against the codebase, and drafting evidence-based assessments for humans to act on.

**What you'll create.** Before any agent exists, you'll build a replay harness: a curated collection of historical reports with known outcomes (confirmed, rejected, duplicate), plus simple baselines such as rule-based filters and embedding-based duplicate detection. The agent must then beat those baselines on replayed history. Ultimately, the goal is to create a working open source tool, an evaluation report, a security analysis against a recognized risk framework, and documented design reviews with practitioners. This gives employers evidence you can perform system design, evaluation, security analyses, and stakeholder communication.

**Need.** 3 to 5 students. Python required. Experience with TypeScript, interest in security, APIs, human-computer interaction, and an interest in communicating with practitioners useful.

## Track 3: The Interpretive Bottleneck

**Overview.** Why does adding capable AI to a group sometimes make the group worse? The curl example has a clear abstract structure: producing visible work became nearly free, interpreting it stayed costly and human, and the group's interpretive capacity became the bottleneck. You will build a model that explains when this happens and what changes the outcome.

**What you'll create.** An agent-based simulation model in which tasks vary in how easy they are to interpret, agents vary in interpretive ability, and producing visible artifacts is cheap while interpreting them is costly. Before the model is used to make any new claims, it must reproduce three quantified patterns from real data: reduced the falling signal rate in the curl case (roughly one valid report in twenty by late 2025), the load concentration found by Census III (one or two people carrying over 80 percent of contributions in 40 percent of top projects), and the maintainer exit pattern seen in cases like Ingress NGINX. Then the model does its real job: comparing interventions. Which policies (filtering, making submissions costly, adding interpretive capacity, redistributing load) delay or prevent collapse, and at what cost? Two interfaces make this concrete. Track 1's accuracy results estimate your AI agents' interpretive-ability parameters, and Track 2's Sentinel enters your comparison as one implemented intervention, so your model makes a prediction their system can check. The aim is to produce an open, tested simulation codebase, a validation report against real-world data, an intervention comparison with practical implications, and a public interactive visualization that communicates to technical and non-technical audiences alike.

**Need.** 3 to 5 students. Python required. Useful: simulation or statistics background, and one member comfortable with light front-end work. No prior agent-based modeling experience required.

## How the Tracks Connect: Interfaces

TBD

## Who Should Apply

You should apply if you're interested in practicing the following:

- **Decision-making amidst ambiguity.** Working on unsolved problems (like this) creates opportunities for you to practice making decisions amidst ambiguity. Sometimes we will not know the right answer, or there will not be a right answer at all. You don't need to be comfortable with ambiguity—most people aren't, including me! But practicing making decisions with supporting evidence on a project like this will make it easier, though.

- **Workplace Application of AI Models.** Whether you love AI or hate AI, you will learn what the frontier AI models can and cannot do in organizational contexts, even as capabilities evolve. What workplace activities do AIs do well, and where do they fall short? How can we bridge the gap? This is evolving, and you'll help us figure all of this out.

- **Teamwork.** The best companies *only* hire people who work well in teams. This project will help you prove that you can do this. You'll practice teamwork by giving each other regular (kind) feedback, carefully deciding interface requirements together, communicating about deliverables, and holding each other accountable.

Python is our working language. Prior experience with AI systems, security, simulation, or open source is useful but not required. Willingness to learn in public is required.

## Attendance

- One all-hands meeting every two weeks (about an hour) where each track shares progress, decisions, and blockers. Gate rehearsals happen here.

- One weekly track check-in with me, scheduled per team in the first week of class. In these meetings, I don't need you to prove to me that you're making progress – that's what the gates are for. Instead, these are for you. What do you need? What questions do you have? What do you want feedback on? Just come prepared with something to discuss that helps your team advance toward its goal.

## Grading Criteria

Each semester, you will earn credit for successful gate reviews, peer evaluations, and a self-assessment. An ambitious attempt that partially fails, with a clear account of what you learned, is worth more than a safe attempt that fully succeeds.

- **50% Gate Reviews (by track).** Two stage gate reviews, weighted 20% and 30% respectively. You will present what you decided and why, what you learned and built, and what you tried and abandoned. Failure and success can both earn credit as long as your team provides evidence.

- **30% Peer Evaluations.** Members of the other tracks will evaluate what your track produced. Other members of your team will evaluate what you produced.

- **20% Self Assessment.** What you contributed, what you did well, what you did not do as well as you wanted, what you would do differently, what you can do in your next role.

## How we Work Together

All project work is developed in the [Invisible Work Initiative's repositories](https://github.com/invisible-work-initiative) under open licenses. Joining the project means you agree to work this way. Our primary language is Python, but we'll use other languages as needed. Code will be fully reproducible. All work goes into public repositories under open licenses from the start, not at the end. You will experience both the benefits and the frictions of working in the open. Each gate deliverable must be reproducible by a teammate from the repository alone. If it only runs on your laptop, it does not exist. AI tools are permitted and expected. You are accountable for everything you submit. Submitting unverified generated work that others must review is the exact failure this initiative exists to address.
