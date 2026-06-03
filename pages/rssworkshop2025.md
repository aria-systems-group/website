---
title: RSS Workshop on <br> <b>Planning and Control with Imperfect Sensors and Perception</b> 
layout: page 
permalink: /workshops/planning-perception.html
class: no-nav
---
<nav class="workshop-nav">
  <a href="#about" class="nav-toggle">About</a>
  <a href="#call-for-papers" class="nav-toggle">Call for papers</a>
  <a href="#important-dates" class="nav-toggle">Important dates</a>
  <a href="#organizers" class="nav-toggle">Organizers</a>
  <a href="#invited-speakers" class="nav-toggle">Invited Speakers</a>
  <a href="#program" class="nav-toggle">Program</a>
</nav>

<style>
  .workshop-nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    /*gap: 4px;*/
    padding: 6px 0;
    margin: 6px 0;
    border-top: 1px solid #e0e0e0;
    border-bottom: 1px solid #e0e0e0;
  }
  .nav-toggle {
    /*display: inline-block;
    padding: 8px 18px;
    font-size: 14px;
    font-weight: 500;
    color: #2c3a4f;
    background: #f5f5f5;
    border: 1px solid #d8d8d8;
    border-radius: 20px;
    text-decoration: none;
    transition: background 0.15s, color 0.15s;*/
    padding: 6px 28px;
    font-size: 14px;
    font-weight: 500;
    color: #2c3a4f;
    background: #f5f5f5;
    border: 0.5px solid #d8d8d8;
    border-radius: 0.5px;
    text-decoration: none;
    text-align: center;
    transition: background 0.15s, color 0.15s;
  }
  .nav-toggle:hover {
    background: #2c3a4f;
    color: #fff;
    border-color: #2c3a4f;
  }
  /* Offset the scroll position so the heading isn't hidden under any fixed header */
  #about, #call-for-papers, #important-dates, #invited-speakers, #organizers {
    scroll-margin-top: 24px;
  }
</style>

<style>
  .people-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 24px;
    margin: 24px 0 32px 0;
  }

  .person-card {
    text-align: center;
    padding: 18px;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    background: #fafafa;
  }

  .person-card img {
    width: 150px;
    height: 150px;
    object-fit: cover;
    border-radius: 50%;
    margin-bottom: 12px;
    border: 1px solid #ddd;
  }

  .person-card h3 {
    margin: 8px 0 4px 0;
    font-size: 18px;
  }

  .person-card p {
    margin: 2px 0;
    font-size: 14px;
    line-height: 1.35;
  }

  .person-card .role {
    font-weight: 500;
    color: #2c3a4f;
  }

  .person-card .tbd-face {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: #eeeeee;
    border: 1px solid #ddd;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 12px auto;
    color: #777;
    font-size: 18px;
    font-weight: 500;
  }
</style>

<figure>
  <img src="/assets/images/rssworkshopbanner2.jpg" alt="Planning and Control with Imperfect Sensors and Perception">
</figure>
<!-- <div style="display: flex; justify-content: space-around; text-align: center;"> -->
  <!-- <div><span class="meta-icon">🗒</span> July 17, 2026</div> -->
  <!-- <div><span class="meta-icon">🕐</span> Submissions due June 5</div> -->
  <!-- <div><span class="meta-icon">📄</span> 2-page extended abstract</div> -->
  <!-- <div><span class="meta-icon">📤</span> <a href="https://openreview.net/group?id=roboticsfoundation.org/RSS/2026/Workshop/WPCIS">Submit here</a></div> -->
<!-- </div> -->

<!-- <br> -->
<!-- **Title:**  -->

<!-- **<span style="color:blue">Description</style>** -->

<!-- <span style="color:black"> -->

<!-- ## This workshop is cancelled

**We are sad to say that the workshop will not take place as part of RSS this year.  Many of the invited speakers are unfortunately unable to attend the workshop in person.  Since that affects the quality of the workshop, we decided to postpone it to another conference to ensure that the workshop will be productive with a good turnout.  We will soon make an announcement which conference we will target next.** -->

<!-- <br> -->

<!-- As autonomous robotic systems transition from controlled labs to unstructured, high-stakes environments, the traditional decoupling between perception, planning, and control is becoming untenable. Imperfections in these subsystems are inescapable byproducts of operating in the physical world. Failure to account for them leads to overconfident behaviors, where a robot assumes an accurate world state despite partial or imperfect measurements and observations. In safety-critical settings, this can result in catastrophic failures, such as collisions with unseen obstacles or loss of localization or tracking in feature-poor areas.

Yet, properly accounting for sensors and their imperfections is notoriously difficult. Tightly coupling perception, planning and control requires reasoning over very high-dimensional problem spaces, which is often computationally prohibitive for real-time applications. Additionally, accurate modeling of sensor and perception uncertainty is complicated due to the increasingly black-box nature of modern perception stacks.

This workshop addresses the critical need for techniques that account for imperfect perception during planning. Our focus is on strategies where robots do not just react to sensory data, but actively plan by reasoning over sensory information and limitations (e.g., neural network labeling faults or field-of-view constraints). Particular emphasis is on robust techniques with safety considerations. The objective is to gather researchers and practitioners in the broad area of perception-aware autonomy. We attempt to highlight recent advances in these communities, discuss open problems and main challenges, and lay out new research directions. -->

<h2 id="about">Overview</h2>

Autonomous robotic systems are increasingly deployed in unstructured, open-world, and safety-critical environments, where sensing and perception are inherently imperfect. Classical modular autonomy pipelines often assume that perception provides a sufficiently accurate state estimate for planning and control. In practice, however, robots must operate under partial observability, uncertain semantic information, limited fields of view, noisy localization, and perception modules that may degrade under distribution shift.

At the same time, modern perception systems are shifting from geometric state estimation toward richer, semantic and language-conditioned representations. Advances in vision-language models (VLMs), vision-language-action (VLA) systems, and large-scale multimodal learning enable robots not only to recognize objects, but to reason about context, relationships, and the implications of their actions. These developments introduce new opportunities for more general and context-aware autonomy, but also raise fundamental challenges: how should such high-dimensional, semantic, and often uncertain representations interface with planning and control? How can semantic reasoning be translated into actionable decisions with reliability and safety guarantees? These developments blur the boundary between perception and decision-making, making the design of their interface a central challenge.

This workshop examines emerging challenges in tightly coupled perception, planning, and control under these new conditions. In particular, we focus on settings where decision-making must operate over uncertain, high-dimensional, and semantically structured representations, rather than well-defined state estimates. We are interested in both modular and end-to-end approaches, and the trade-offs between explicit modeling of uncertainty and implicit reasoning in learned systems. The workshop will bring together researchers from robotics, machine learning, controls, formal methods, and field robotics to foster interdisciplinary discussion on perception-aware autonomy. Our goal is to identify key open problems at the interface of perception and decision-making, evaluate emerging paradigms enabled by modern learned perception, and outline principled directions for building reliable autonomous systems in the real world.

<!-- <br> -->


### Discussion Questions

- How should uncertainty from perception—especially from learned and semantic models—be represented and incorporated into planning and control?

- How can high-dimensional perception outputs be translated into representations, constraints, and objectives for decision-making?

- What representations best support both reasoning and control (e.g., belief states, scene graphs, latent/world models), and how should they be constructed?

- How do we reason about context, interactions, and temporal dynamics in perception-aware planning?

- How do learned planning and control methods interact with learned perception, and what new challenges arise when both perception and decision-making are data-driven?

- What new failure modes arise from modern learned perception systems (e.g., hallucination, distribution shift), and how should decision-making and control systems account for them?

- What are the trade-offs between modular pipelines and end-to-end learning approaches in perception, planning, and control?

- What is the role of formal guarantees and verification when perception is uncertain, learned, and semantically rich?

- How should we evaluate perception-aware autonomy? What benchmarks, datasets, and metrics are needed to measure reliability and safety in real-world deployment?

<hr>

<h2 id="call-for-papers">Call for Papers</h2>

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

We welcome both ongoing work and recently published results. Accepted contributions will be presented as posters during the workshop, with selected submissions invited for spotlight talks. All accepted abstracts and posters will be made publicly available on the workshop website. This is a non-archival venue, and submissions may be published elsewhere. Abstracts should be a maximum of **2 pages** long (excluding references) in RSS paper format ([LaTeX](https://roboticsconference.org/docs/paper-template-latex.tar.gz)). 

- **Submission link:** [https://openreview.net/group?id=roboticsfoundation.org/RSS/2026/Workshop/WPCIS](https://openreview.net/group?id=roboticsfoundation.org/RSS/2026/Workshop/WPCIS).

<hr>
<h3 id="important-dates">Important Dates</h3>
- Abstract submission: June 5, 2026 (11:59pm <a href="https://time.is/Anywhere_on_Earth">AoE</a>)
- Notification: June 12, 2026
- Workshop: July 17, 2026


<!--## Tentative Schedule

- 8:45 - 9:00 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Welcome and Introduction
- 9:00 - 9:30 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 1 
- 9:30 - 10:00 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 2 
- 10:00 - 10:30	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 3
- 10:30 - 11:00	&nbsp;&nbsp;&nbsp;&nbsp; Coffee Break (poster session)
- 11:00 - 11:30	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 4
- 11:30 - 12:00	&nbsp;&nbsp;&nbsp;&nbsp; Invited Speaker 5
- 12:00 - 12:15	&nbsp;&nbsp;&nbsp;&nbsp; Poster Spotlight Talks
- 12:15 - 13:00	&nbsp;&nbsp;&nbsp;&nbsp; Panel Discussion and Debate-->


<!--## Invited Speakers and Panelists

- [Hannah Kurniawati](hanna.kurniawati@anu.edu.au), Professor, Australian National University 
- [Yiannis Kantaros](ioannisk@wustl.edu) (confirmed), Assistant Professor, Washington University in St. Louis
- And more TBD-->

<hr>

<h2 id="invited-speakers">Invited Speakers and Panelists</h2>

<div class="people-grid">

  <div class="person-card">
    <img src="/assets/images/hanna-kurniawati.jpg" alt="Hanna Kurniawati">
    <h3><a href="https://comp.anu.edu.au/people/hanna-kurniawati/">Hanna Kurniawati</a></h3>
    <p class="role">Professor</p>
    <p>Australian National University</p>
  </div>

  <div class="person-card">
    <img src="/assets/images/Yiannis-Kantaros1.jpg" alt="Yiannis Kantaros">
    <h3><a href="https://engineering.washu.edu/faculty/Yiannis-Kantaros.html">Yiannis Kantaros</a></h3>
    <p class="role">Assistant Professor</p>
    <p>Washington University in St. Louis</p>
  </div>

  <div class="person-card">
    <img src="/assets/images/talak_people.jpg" alt="Rajat Talak">
    <h3><a href="https://www.rajattalak.com/">Rajat Talak</a></h3>
    <p class="role">Assistant Professor</p>
    <p>National University of Singapore</p>
  </div>

  <div class="person-card">
    <img src="/assets/images/jon_decastro.png" alt="Jonathan DeCastro">
    <h3><a href="https://jadecastro.github.io">Jonathan DeCastro</a></h3>
    <p class="role">Research Scientist</p>
    <p>Toyota Research Institute</p>
  </div>

</div>

<hr>

<h2 id="organizers">Organizers</h2>

<div class="people-grid">

  <div class="person-card">
    <img src="/assets/images/qihengho.jpg" alt="Qi Heng Ho">
    <h3><a href="https://www.aoe.vt.edu/people/faculty/qi-heng-ho.html">Qi Heng Ho</a></h3>
    <p class="role">Assistant Professor</p>
    <p>Virginia Tech</p>
  </div>

  <div class="person-card">
    <img src="/assets/images/Malika%20Meghjani%20Profile.jpg" alt="Malika Meghjani">
    <h3><a href="https://www.malikameghjani.com/">Malika Meghjani</a></h3>
    <p class="role">Assistant Professor</p>
    <p>Singapore University of Technology and Design</p>
  </div>

  <div class="person-card">
    <img src="/assets/images/morteza-lahijanian-200.jpeg" alt="Morteza Lahijanian">
    <h3><a href="https://www.colorado.edu/aerospace/morteza-lahijanian">Morteza Lahijanian</a></h3>
    <p class="role">Associate Professor</p>
    <p>University of Colorado Boulder</p>
  </div>

</div>

For inquiries, please contact: [rss2026wpcis@gmail.com](mailto:rss2026wpcis@gmail.com)


<hr>

<h2 id="program">Program</h2>
All times are <em>local</em> to the conference venue (July 17, 2026).

<!-- <table style="width:100%; border-collapse: collapse;">
  <thead>
    <tr style="border-bottom: 2px solid #333;">
      <th style="text-align:left; padding: 8px;">Time</th>
      <th style="text-align:left; padding: 8px;">Session</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="padding: 8px;">2:00 – 2:10</td><td style="padding: 8px;">Opening remarks</td></tr>
    <tr><td style="padding: 8px;">2:10 – 2:40</td><td style="padding: 8px;">Invited Speaker 1</td></tr>
    <tr><td style="padding: 8px;">2:40 – 3:10</td><td style="padding: 8px;">Invited Speaker 2</td></tr>
    <tr><td style="padding: 8px;">3:10 – 3:20</td><td style="padding: 8px;">Lightning Talks</td></tr>
    <tr><td style="padding: 8px;">3:20 – 3:50</td><td style="padding: 8px;">Coffee break and poster session</td></tr>
    <tr><td style="padding: 8px;">3:50 – 4:20</td><td style="padding: 8px;">Invited Speaker 3</td></tr>
    <tr><td style="padding: 8px;">4:20 – 4:50</td><td style="padding: 8px;">Invited Speaker 4</td></tr>
    <tr><td style="padding: 8px;">4:50 – 5:50</td><td style="padding: 8px;">Panel discussion / debate</td></tr>
    <tr><td style="padding: 8px;">5:50 – 6:00</td><td style="padding: 8px;">Closing remarks</td></tr>
  </tbody>
</table> -->


<table class="schedule">
  <thead>
    <tr>
      <th>Time</th>
      <th>Session</th>
    </tr>
  </thead>
  <tbody>
    <tr class="highlight">
      <td class="time">2:00 – 2:10 PM</td>
      <td>Opening remarks</td>
    </tr>
    <tr>
      <td class="time">2:10 – 2:40 PM</td>
      <td>Invited Talk 1</td>
    </tr>
    <tr>
      <td class="time">2:40 – 3:10 PM</td>
      <td>Invited Talk 2</td>
    </tr>
    <tr>
      <td class="time">3:10 – 3:20 PM</td>
      <td>Lightning Talks</td>
    </tr>
    <tr class="break">
      <td class="time">3:20 – 3:50 PM</td>
      <td>Coffee break &amp; poster session</td>
    </tr>
    <tr>
      <td class="time">3:50 – 4:20 PM</td>
      <td>Invited Talk 3</td>
    </tr>
    <tr>
      <td class="time">4:20 – 4:50 PM</td>
      <td>Invited Talk 4</td>
    </tr>
    <tr class="highlight">
      <td class="time">4:50 – 5:50 PM</td>
      <td>Panel discussion &amp; debate</td>
    </tr>
    <tr class="highlight">
      <td class="time">5:50 – 6:00 PM</td>
      <td>Closing remarks</td>
    </tr>
  </tbody>
</table>
