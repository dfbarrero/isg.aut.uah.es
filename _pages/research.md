---
title: Research
layout: single
permalink: /research/
header:
  overlay_image: /assets/img/puente.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
  #cta_label: "More Info"
  #cta_url: "https://unsplash.com"
---

<style>
img[src$="centerme"] {
   display:block;
   margin: 0 auto;
}
</style>

![ISG lab]({{site.baseurl}}/assets/img/lab4.jpg?style=centerme "ISG lab")

Planning & Scheduling solutions for optimal tasks allocation in complex scenarios such as the science program of a spacecraft. We employ technologies for modelling the scenarios such as PDDL or DDL (used by ESA in various projects) for dealing with resources and temporal constraints. So, we have expertise in both action-oriented and timelines-based system, being able to determine which is better for each application. For implementing the solvers we use techniques such as HTN, heuristic search and, more recently, genetic algorithms. 

Path planning and navigation for robotics systems, specially focused (but not limited to) surface robotics. We have developed path planning algorithms for robots with limited turning capabilities or those who have to deal with complex terrains, such as the Mars surface. In this direction, we successfully deployed an algorithm that enables slope-limited paths and hazardous areas avoidance during the path extraction. As well, our path planning algorithms are integrated into a task planning (exploiting the previously mentioned Planning & Scheduling solutions) system to generate optimal solutions when facing multiple goals in different locations. 

![LARES project motes]({{site.baseurl}}/assets/img/lab1.jpg?style=centerme "LARES project motes")

We create autonomous controllers for robotics based on our previous assets. By integrating Planning & Execution engines, we can deploy autonomous robots that are able to deal with uncertainty and dynamic environments. We have experience in GOAC, an autonomous controller developed for ESA. In this regard, we exploit Planning & Scheduling to model and solve high level abstractions of the robot environment and capabilities, technologies such PLEXIL (developed by NASA) or T-REX (based on IDEA, also developed by NASA) for the Planning & Execution integration and functional layers such as ROS or GenOM (used by ESA in the GOAC controller) for the robot hardware abstraction layer. In order to perform real test of such autonomous controllers, we are developing an Unmanned Aerial Vehicle (UAV) which integrates the planning & execution engines with the functional layer of the UAV.

Related to the last one, we have an open research line in assessing autonomous controllers with the objective of Verifying & Validating autonomous robots, an activity started in a PhD program funded by ESA. In this sense our objective is to create a common framework to enhance the trust in autonomous systems with a particular focus on the space exploration. This framework allows us to exhaustively test autonomous controllers in different circumstances, characterizing different behaviours while assessing the performance and identifying flaws that are hardly to observe otherwise. 

![ISG staff working]({{site.baseurl}}/assets/img/lab2.jpg?style=centerme "ISG staff working")

We are pursuing to integrate all these systems into a Virtual Reality framework in which we can evaluate the solutions proposed by the different Planning & Scheduling systems and to observe the execution of autonomous controllers. Also, this opens a research line in Human Machine Interface, in which we face how to interact with autonomous agents in a natural way. This last research line is aligned with ESA objectives of using those techniques for operational procedures by astronauts and spacecraft operators.

![Robotic arm]({{site.baseurl}}/assets/img/lab3.jpg?style=centerme "Robotic arm")

We also face the robotic cooperation for future exploration missions in which we want to explore a large area of a planet by means of an autonomous rover and an aerial vehicle. Both robots have to cooperate to successfully achieve their objectives; while the rover has limited mobility but high battery capacity, the aerial vehicle can cover long distances faster, but requiring to recharge its battery through the rover. In order to support this cooperation approach, we are building a simulation environment on the Virtual Robot Experimentation Platform (V-REP).

![ISG staff]({{site.baseurl}}/assets/img/lab6.jpg?style=centerme "ISG staff")

Low-cost solutions for sensor arrays deployment. Currently we have developed a low-cost wireless sensor network with low energy consumption algorithms. At this very moment, this sensor is coupled to an autonomous robot in a telecare assistance application. Notwithstanding, we are developing wearables devices for health monitor that can be coupled with the telecare system. In this sense, we have expertise in real-time operating systems, PCB design and DAQ systems. 

