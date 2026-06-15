---
layout: home
title: The Invisible Work Initiative
---

***Can AI recognize and perform the work that keeps software working?***

Software of all kinds depends on work that few people see. Reviewing bug reports, judging their severity, detecting duplicates, mentoring newcomers, and deciding what a confusing request is really asking for are all examples of this. Tasks like these keep critical software operating, but they rarely leave the kind of visible record that code does. This is called [invisible work](https://dl.acm.org/doi/10.1145/3757417).

For years, open source workers (in software and other fields) have been straining under invisible workloads. Unfortunately, generative AI has largely added to this volume of work to date. For instance:

- [Census III](https://www.linuxfoundation.org/press/open-source-usage-trends-and-security-challenges-revealed-in-new-study), by the Linux Foundation and Harvard, found that 40 percent of the most widely used open source projects depend on one or two developers for more than 80 percent of contributions. This makes them vulnerable to attacks and growth of AI submissions.
- In November 2025, [Kubernetes retired Ingress NGINX](https://www.kubernetes.io/blog/2026/01/29/ingress-nginx-statement/), a component used in roughly half of cloud computing environments. Development had fallen to one or two people working in their spare time; no replacements could be found.
- In January 2026, curl, a widely-used data transfer program, [ended its bug bounty program](https://www.theregister.com/2026/01/21/curl_ends_bug_bounty/) due to an influx of AI-generated vulnerability reports. curl's small volunteer security team couldn't keep up. Django, Node.js, and libxml2 restricted their intake processes for the same reason.
- Meanwhile, benchmarks for AI coding agents, such as the [SWE-bench](https://arxiv.org/abs/2310.06770) family, measure whether an agent can produce a code patch that resolves an issue. None of them measure the judgment work described above.

<figure style="margin: 1.5rem 0; text-align: center;">
  <img src="https://imgs.xkcd.com/comics/dependency.png" alt="XKCD comic no. 2347, 'Dependency'." style="max-width: 100%; height: auto;" />
  <figcaption style="font-size: 0.85em; color: #6f6f6f; margin-top: 0.5rem;"><a href="https://xkcd.com/2347/">XKCD</a>. A bit reductive, but true in spirt!</figcaption>
</figure>

The thesis of this initiative: AI systems produce vast amounts of visible work. But small numbers of humans perform the invisible work of judging and coordinating work with stakeholders. Humans alone cannot keep up with AI products. This asymmetry is breaking organizations and computing infrastructure.

We address this challenge through two-semester M.Eng. projects in the Systems Engineering Program at Cornell University, advised by Prof. John Meluso, PhD. Coordinated student teams will design systems to make open source ecosystems better for everyone involved.

## Get involved

- **Read the [AI for Open Source Bug Reports project syllabus](/projects/ai-for-open-source-bug-reports/)** for the full description, teams, and expectations.
- **Apply to join** through the [project application form](https://forms.gle/x56KEJ5Pex9PAeTU9).
- **Follow the work** in our [GitHub organization](https://github.com/invisible-work-initiative). All work is developed in the open under open licenses from the start.
