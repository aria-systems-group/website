---
name: Expert-Informed Autonomous Science Planning for In-situ Observations and Discoveries                               # Name
title: Expert-Informed Autonomous Science Planning for In-situ Observations and Discoveries     
layout: project                     # Leave it as it is
ordering: 2                          # Order to be appeared in the page
status: current                            # Choose either current or past
picture:                            # Path to the image file
excerpt_separator: <!--more-->
link-flag: true                          # Choose either true or false
bibkey: coldtech                             # Unique key that relates the project to some bibfiles
---

In this project, we are developing a framework to maximize science obtained by robotic landers in future space missions on the surface of distant bodies such as Europa. The key challenges we address is to reduce the dependency of human-in-the-loop operations and changes in the environment for limited-time missions by developing correct-by-construction algorithmic approaches that integrate formal method, game theory, and control theory.

<!--more-->

<img class="center" src="{{site.baseurl}}/assets/images/projects/coldtech/architecture_overview.png" alt="full_plan" width="600px"/>
<p style="text-align:center">The proposed framework.</p>

Future planetary exploration missions on the surface of distant bodies such as Europa or Enceladus can’t rely on human-in-the-loop operations due to time delays, dynamic environments, limited mission lifetimes, as well as the many unknown unknowns inherent in the exploration of such environments.

In this project, we are developing a framework to maximize the science obtained by a robotic lander and delivered to scientists on Earth with minimal asynchronous human interaction. The autonomy architecture consists of three main components: Shared Science Value Maps (SSVMs), which function as an interface between REASON (Robust Exploration with Autonomous Science on-board) and RECOURSE (Ranked Evaluation of Contingent Opportunities for Uninterrupted Remote Science Exploration) for efficient and useful scientific communication between scientists and robot as shown in the Figure. The key advantage to this design is its ability to react and adapt to dynamic environments. 

Our lab focuses on developing REASON, an on-board opportunistic planner that works in synergy with the SSVM to maximize science that reaches earth. We use formal methods to design, express, and implement our science activities and develop novel task-and-motion planners to ensure the proper functionality of REASON to engender trust and provide assurances in the system’s performance. 
