---
name: Explainable Multi-Agent Planning
title: Explainable Multi-Agent Planning
layout: project
ordering: 1
status: current
picture:
images:
- url: /assets/images/projects/ma-paths/path-segs.png
excerpt_separator: <!--more-->
link-flag: true
bibkey: ma-planning
---

As we begin employing teams of robots to accomplish complex tasks, it becomes difficult for a human to verify that future paths do not result in collisions. Therefore, we are working on new multiagent planning approaches that minimize the effort it takes a human to verify the paths.

<!--more-->

<img class="center" src="{{site.baseurl}}/assets/images/projects/ma-paths/fullPlan.png" alt="full_plan" width="200px"/>
<p style="text-align:center">Full plan for three agents</p>
<img class="center" src="{{site.baseurl}}/assets/images/projects/ma-paths/seg1-3.png" alt="segments" width="600px"/>
<p style="text-align:center">Explanations of the full plan in 3 parts for quick validation</p>

As we begin employing teams of robots to accomplish complex tasks, it becomes difficult for a human to verify that future paths do not result in collisions. Therefore, we are working on new multiagent planning approaches that minimize the effort it takes a human to verify the paths.

Multi-agent motion planning (MMP) is the problem of finding a motion plan for multiple agents such that when these agents are run simultaneously, none of the agents collide. These motion plans are traditionally computed using provably correct algorithms and immediately executed on a real system. In safety-critical applications, however, a human supervisor may want to verify that the plan is indeed collision-free prior to execution. This process can be extremely unintuitive since MMP solutions commonly have intersecting lines, making it difficult to verify that the agents do not collide. The inability for humans to validate traditional MMP algorithms leaves a huge trust-gap between motion planning experts and the daily-users who could benefit from using such algorithms. This work focuses on shortening the gap by incorporating explainability into traditional MMP algorithms.

We investigate the notion of an explanation for a plan of MMP, based on visualization of the plan as a short sequence of images representing time segments, where in each time segment the trajectories of the agents are disjoint, clearly illustrating the safety of the plan. Presenting the plan in this way makes it very easy for a human to recognize the plan is collision free because recognizing line intersections happens very early in the cognitive process. Giving MMP algorithms the ability to explain their solutions to humans would greatly shorten the trust-gap between motion planning research experts and daily-users of these algorithms, consequentially allowing MMP algorithms to be further utilized within safety-critical systems.

