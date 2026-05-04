---
title: RSS Workshop on <br> Planning and Control with Imperfect Sensors and Perception 
layout: page 
permalink: /workshops/planning-perception.html
class: no-nav
---



<br>
<!-- **Title:**  -->

<!-- **<span style="color:blue">Description</style>** -->

<!-- <span style="color:black"> -->

<!-- ## This workshop is cancelled

**We are sad to say that the workshop will not take place as part of RSS this year.  Many of the invited speakers are unfortunately unable to attend the workshop in person.  Since that affects the quality of the workshop, we decided to postpone it to another conference to ensure that the workshop will be productive with a good turnout.  We will soon make an announcement which conference we will target next.** -->

<br>

<!-- As autonomous robotic systems transition from controlled labs to unstructured, high-stakes environments, the traditional decoupling between perception, planning, and control is becoming untenable. Imperfections in these subsystems are inescapable byproducts of operating in the physical world. Failure to account for them leads to overconfident behaviors, where a robot assumes an accurate world state despite partial or imperfect measurements and observations. In safety-critical settings, this can result in catastrophic failures, such as collisions with unseen obstacles or loss of localization or tracking in feature-poor areas.

Yet, properly accounting for sensors and their imperfections is notoriously difficult. Tightly coupling perception, planning and control requires reasoning over very high-dimensional problem spaces, which is often computationally prohibitive for real-time applications. Additionally, accurate modeling of sensor and perception uncertainty is complicated due to the increasingly black-box nature of modern perception stacks.

This workshop addresses the critical need for techniques that account for imperfect perception during planning. Our focus is on strategies where robots do not just react to sensory data, but actively plan by reasoning over sensory information and limitations (e.g., neural network labeling faults or field-of-view constraints). Particular emphasis is on robust techniques with safety considerations. The objective is to gather researchers and practitioners in the broad area of perception-aware autonomy. We attempt to highlight recent advances in these communities, discuss open problems and main challenges, and lay out new research directions. -->

## Overview

Autonomous robotic systems are increasingly deployed in unstructured, open-world, and safety-critical environments, where sensing and perception are inherently imperfect. Classical modular autonomy pipelines often assume that perception provides a sufficiently accurate state estimate for planning and control. In practice, however, robots must operate under partial observability, uncertain semantic information, limited fields of view, noisy localization, and perception modules that may degrade under distribution shift.

At the same time, modern perception systems are shifting from geometric state estimation toward richer, semantic and language-conditioned representations. Advances in vision-language models (VLMs), vision-language-action (VLA) systems, and large-scale multimodal learning enable robots not only to recognize objects, but to reason about context, relationships, and the implications of their actions. These developments introduce new opportunities for more general and context-aware autonomy, but also raise fundamental challenges: how should such high-dimensional, semantic, and often uncertain representations interface with planning and control? How can semantic reasoning be translated into actionable decisions with reliability and safety guarantees? These developments blur the boundary between perception and decision-making, making the design of their interface a central challenge.

This workshop examines emerging challenges in tightly coupled perception, planning, and control under these new conditions. In particular, we focus on settings where decision-making must operate over uncertain, high-dimensional, and semantically structured representations, rather than well-defined state estimates. We are interested in both modular and end-to-end approaches, and the trade-offs between explicit modeling of uncertainty and implicit reasoning in learned systems. The workshop will bring together researchers from robotics, machine learning, controls, formal methods, and field robotics to foster interdisciplinary discussion on perception-aware autonomy. Our goal is to identify key open problems at the interface of perception and decision-making, evaluate emerging paradigms enabled by modern learned perception, and outline principled directions for building reliable autonomous systems in the real world.

<br>


## Discussion Questions

- How should uncertainty from perception—especially from learned and semantic models—be represented and incorporated into planning and control?

- How can high-dimensional perception outputs be translated into representations, constraints, and objectives for decision-making?

- What representations best support both reasoning and control (e.g., belief states, scene graphs, latent/world models), and how should they be constructed?

- How do we reason about context, interactions, and temporal dynamics in perception-aware planning?

- How do learned planning and control methods interact with learned perception, and what new challenges arise when both perception and decision-making are data-driven?

- What new failure modes arise from modern learned perception systems (e.g., hallucination, distribution shift), and how should decision-making and control systems account for them?

- What are the trade-offs between modular pipelines and end-to-end learning approaches in perception, planning, and control?

- What is the role of formal guarantees and verification when perception is uncertain, learned, and semantically rich?

- How should we evaluate perception-aware autonomy? What benchmarks, datasets, and metrics are needed to measure reliability and safety in real-world deployment?


## Call for Papers

We invite submissions of extended abstracts to share novel ideas on topics relevant to the workshop themes, which include but are not limited to:

- Planning and control under sensing uncertainty
- Vision-based and learned perception (including VLM/VLAs)
- Active perception and information gathering
- Context-aware and semantic planning and control
- Classification, object, and semantic uncertainty 
- Partially Observable Markov Decision Processes
- Sim-to-real transfer and uncertainty quantification
- Multi-agent interaction with semantic information
- Learned planning and control

We welcome both ongoing work and recently published results. Accepted contributions will be presented as posters during the workshop, with selected submissions invited for spotlight talks. All accepted abstracts and posters will be made publicly available on the workshop website. This is a non-archival venue, and submissions may be published elsewhere. Abstracts should be a maximum of 2 pages long in RSS paper format.

### Important Dates
- Abstract submission: May 24, 2026
- Notification: June 7, 2026
- Workshop: July 17, 2026

Submissions should be made to OpenReview 


## Tentative Schedule

- 8:45 - 9:00 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Welcome and Introduction
- 9:00 - 9:30 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 1 
- 9:30 - 10:00 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 2 
- 10:00 - 10:30	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 3
- 10:30 - 11:00	&nbsp;&nbsp;&nbsp;&nbsp; Coffee Break (poster session)
- 11:00 - 11:30	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 4
- 11:30 - 12:00	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 5
- 12:00 - 12:15	&nbsp;&nbsp;&nbsp;&nbsp; Poster Spotlight Talks
- 12:15 - 13:00	&nbsp;&nbsp;&nbsp;&nbsp; Panel Discussion and Debate


<!--## Invited Speakers and Panelists

- [Hannah Kurniawati](hanna.kurniawati@anu.edu.au), Professor, Australian National University 
- [Yiannis Kantaros](ioannisk@wustl.edu) (confirmed), Assistant Professor, Washington University in St. Louis
- And more TBD-->


## Organizers

- **[Qi Heng Ho](https://www.aoe.vt.edu/people/faculty/qi-heng-ho.html)**<br>
Assistant Professor  <br>
Virginia Tech  <br>
<!-- [morteza.lahijanian@colorado.edu](mailto:morteza.lahijanian@colorado.edu)<br> -->

- **[Malika Meghjani](https://www.malikameghjani.com/)** <br>
Assistant Professor  <br>
Singapore University of Technology and Design  <br>
<!-- [angela.schoellig@utoronto.ca](mailto:angela.schoellig@utoronto.ca) -->

- **[Morteza Lahijanian](https://www.colorado.edu/aerospace/morteza-lahijanian)**<br>
Associate Professor  <br>
University of Colorado Boulder  <br>
<!-- [morteza.lahijanian@colorado.edu](mailto:morteza.lahijanian@colorado.edu)<br> -->


