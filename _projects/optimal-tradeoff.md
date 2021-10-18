---
name: "INPASS: Intelligent Navigation, Planning, and Awareness for Swarm Systems"
title: "INPASS: Intelligent Navigation, Planning, and Awareness for Swarm Systems"
layout: project
ordering: 2
status: current
picture:
excerpt_separator: <!--more-->
link-flag: true
bibkey: optimal-tradeoff
---

This project addresses the need to balance competing objectives for multi-agent autonomous systems in exploration of an environment. We aim to provide formal guarantees on performance and resource consumption objectives by using formal analysis techniques.

<!--more-->

This research seeks to address the challenge of generating safe, correct, and verifiable optimal plans. This is achieved by using formal methods to provide guarantees on the objectives studied in an optimal tradeoff analysis. The scenario consists of a set of autonomous agents that can make opportunistic relative measurements of each other (ex. range to other agents, imaging, etc.). These measurements can be communicated with at least some subset of the network. This communication improves state estimation, increasing the probability of satisfying objectives, but also consumes resources. The agents seek to satisfy three mission objectives: 1.) navigate to a goal state, 2.) avoid obstacles, and 3.) minimize resource use. The problem is to find the optimal tradeoff between these competing objectives, which can be captured in a Pareto front. Pareto analysis via formal methods will provide a major advance by allowing users to reason over task objectives rather than implementations.

The novel aspect of this research comes from the application of event triggered estimation. Event-based state estimation is primarily used in systems where resources need to be conserved. Instead of continuously sharing measurements or estimates, the system uses a trigger to decide when new information is worth sharing. There is no analytical method to determine the appropriate threshold for triggering; it must be painstakingly tuned to achieve the desired performance. This research in formal tradeoff analysis offers a way to automatically generate an optimal schedule for the triggering threshold.

If you are interested in learning more, please reach out to Anne Theurkauf at [anne.theurkauf@colorado.edu](mailto:anne.theurkauf@colorado.edu).
