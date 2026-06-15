---
layout: page
title: "Syllabus: AI for Open Source Bug Reports"
permalink: /projects/ai-for-open-source-bug-reports/
---

This project builds one system that addresses part of the open source sustainability challenge: an automated quality checker for incoming bug reports. Several teams build the system together. Each team owns one part and depends on the others' work (see Project Teams).

**Advisor.** Dr. John Meluso, Systems Engineering Program, Cornell University.

**Topics.** Open Source Ecosystems, Human-AI Collaboration, AI Agents, Benchmarking and Evaluation, Data Science, Agent-Based Modeling, Sociotechnical System Design.

**Keywords.** Artificial Intelligence; Invisible Labor; Open Source Sustainability; AI Agents; Benchmarks; Agent-Based Modeling; Human-AI Teaming; Triage.

**Short titles.** AI for OSS, AI for Open Source Bug Reports



## How do I join?

To apply, fill out the project application here (provided before fall semester). You'll be asked to include a resume/CV and some information about yourself! I encourage you to answer in your own words so I can get to know you; don't worry, I don't expect perfect spelling or grammar.

If you receive an invitation to join:

- **Systems Engineering Program.** Complete and submit the SYSEN project form to the program office. Register in the appropriate SYSEN 5900 section (section number to be confirmed before the semester starts).

- **Another Program.** Complete and send me your program's form to sign. Register in an appropriate project section as instructed by your program. Please investigate what your program expects and share what you learn with me. We'll finish the process together.



## Project Teams

This project builds one system: an automated quality checker for incoming bug reports. The teams below build it together. Each team owns one part of the system and depends on the others' work.

**Software Systems Engineering.** This team specifies what the system must do and how we will know it works. You will write a concept of operations, write system-level requirements, verifications, and tests for the integrated system. You will assemble a dataset of historical bug reports from several open source projects and build the test that measures system performance against a standard. You'll be able to show employers that you can lead requirements, verification and validation, and system-level testing on a real system.

**Input Evaluation Subsystem.** This team designs the subsystem that evaluates whether incoming report is worth investigating. You will write requirements, verifications, and tests for your subsystem. Your solution might need to assess if necessary contents are present, such as steps to reproduce and a clear statement of expected versus observed behavior. You'll want to develop familiarity with published research on bug report quality, but also develop awareness of different standards maintainers use to evaluate submitted reports. You'll be able to show employers that you can develop design requirements and create a conforming software solution that interfaces with other subsystems.

**Claim Investigation Subsystem.** This team designs the subsystem that investigates a conforming report. You will write requirements, verifications, and tests for your subsystem. Your solution may need to find relevant files, code, and documentation before comparing their behavior against the report. The lowest-quality reports often cite code or bug that do not exist, or are different than claimed. You'll work directly against real codebases and their version history. You'll be able to show employers that you can develop design requirements and create a conforming software solution that interfaces with other subsystems.

**Integration Subsystem.** This team designs the subsystem that connects the other subsystems and interfaces with the user. You will write requirements, verifications, and tests for your subsystem. Your solution might need to take an incoming report, pass information between subsystems as appropriate, and assemble results into a single report the maintainer sees. As a stretch, you may connect the system to GitHub so that a new issue is reviewed automatically. You'll be able to show employers that you can develop design requirements and create a conforming software solution that interfaces with other subsystems.

## Who Should Apply

**On Campus** and **Distance Learning** students are welcome to apply. You should apply if you're interested in practicing the following:

- **Decision-making amidst ambiguity.** Working on unsolved problems (like this) creates opportunities for you to practice making decisions amidst ambiguity. Sometimes we will not know the right answer, or there will not be a right answer at all. You don't need to be comfortable with ambiguity--most people aren't, including me! But practicing making decisions with supporting evidence on a project like this will make it easier, though.

- **Workplace Application of AI Models.** Whether you love AI or hate AI, you will learn what frontier AI models can and cannot do in organizational contexts, even as capabilities evolve. What workplace activities do AIs do well, and where do they fall short? How can we bridge the gap? This is evolving, and you'll help us figure all of this out.

- **Teamwork.** The best companies *only* hire people who work well in teams. This project will help you prove that you can do this. You'll practice teamwork by giving each other regular (kind) feedback, carefully deciding interface requirements together, communicating about deliverables, and holding each other accountable.

Python is our working language, and some experience is recommended (but not required). Prior experience with AI systems, requirements development, verification and validation, or open source is useful but not required. Willingness to learn in public is required.

## Attendance

- One all-hands meeting every two weeks (about an hour) where each team shares progress, decisions, and blockers. Gate rehearsals happen here.

- One weekly team check-in with me, scheduled per team in the first week of class. In these meetings, I don't need you to prove to me that you're making progress – that's what the gates are for. Instead, these are for you. What do you need? What questions do you have? What do you want feedback on? Just come prepared with something to discuss that helps your team advance toward its goal.

## Grading Criteria

Each semester, you will earn credit for successful gate reviews, peer evaluations, and a self-assessment. An ambitious attempt that partially fails, with a clear account of what you learned, is worth more than a safe attempt that fully succeeds.

- **50% Gate Reviews (by team).** Two stage gate reviews, weighted 20% and 30% respectively. You will present what you decided and why, what you learned and built, and what you tried and abandoned. Failure and success can both earn credit as long as your team provides evidence.

- **30% Peer Evaluations.** Members of the other teams will evaluate what your team produced. Other members of your team will evaluate what you produced.

- **20% Self Assessment.** What you contributed, what you did well, what you did not do as well as you wanted, what you would do differently, what you can do in your next role.

## How we Work Together

I run projects by giving you a goal, targets, and kind, honest feedback. I won't give you instructions on how to reach those goals, though. This means your team gets to make the decisions, write down your reasons, and ask for help when stuck. Yes, you're likely to make lots of mistakes, which is great! *Mistakes are how we learn.* I expect us all to create an environment where everyone feels safe to make mistakes. So you'll experiment, try things, fail sometimes, and try again. An important rule, though: If a problem has blocked you for more than three days, you must seek help (from a teammate, another team, a public forum, an AI assistant). Staying silently stuck is the one form of failure this course does not credit. So help each other and we'll make progress as a team!

All project work is developed in the [Invisible Work Initiative's repositories](https://github.com/invisible-work-initiative) under open licenses. Joining the project means you agree to work this way. Our primary language is Python, but we'll use other languages as needed. Code will be fully reproducible. All work goes into public repositories under open licenses from the start, not at the end. You will experience both the benefits and the frictions of working in the open. Each gate deliverable must be reproducible by a teammate from the repository alone. If it only runs on your laptop, it does not exist. AI tools are permitted and expected. You are accountable for everything you submit. Submitting unverified generated work that others must review is the exact failure this initiative exists to address.