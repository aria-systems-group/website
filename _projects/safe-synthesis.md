---
name: Verifiable Control Synthesis through Model-based Learning with Safety Guarantees
title: Verifiable Control Synthesis through Model-based Learning with Safety Guarantees
layout: project
ordering: 0
status: current
picture:
excerpt_separator: <!--more-->
link-flag: true
bibkey: synth-ml
---

We are combining formal control synthesis and machine learning to tackle uncertainty in autonomous systems applications. By carefully considering the error in the learning process, we aim to develop novel methods for safe control that can adapt to changes in the system and environment.

<!--more-->

Formal control synthesis are *correct-by-construction* approaches to automatically create controllers for autonomous systems.
These controllers aim to accomplish complex tasks specified using temporal logic.
Synthesis is challenging when there is uncertainty in the system, such as the presence of black-box components or incomplete dynamics knowledge, or in the environment.
Machine-learning regression can construct models of these uncertainties that can be used to reason about the future.

Our goal is to combine machine learning regression with formal control synthesis approaches to address these uncertainties.
Mature learning approaches, such as Gaussian process regression, have a strong analytical results that quantify the regression errors.
Our current approach involves constructing abstractions of the system using the learned model, and then use model-based techniques to synthesize a controller.
Ongoing challanges we are investigating include:

* Scalable computational methods for abstraction
* Utilizing other approaches for GP regression and machine learning
* Implementation on robotic systems and vehicles

If you are interested in learning more, please reach out to John Jackson at [john.m.jackson@colorado.edu](mailto:john.m.jackson@colorado.edu) or checkout some of our recent related publications.
