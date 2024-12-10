---
title: "UAV Autonomous Navigation in Dynamic Environments"
# excerpt: "Short description of portfolio item number 1<br/><img src='/images/500x300.png'>"
collection: portfolio
# link: 'https://www.youtube.com/watch?v=UeBShELDzyM'
---

In recent years, lightweight autonomous unmanned aerial vehicles (UAVs) have shown great potential for inspection and mapping in indoor construction sites. However, navigating in indoor environments is complex because of the presence of static and dynamic objects. In this project, we are introducing a navigation framework that enables safe operation in dynamic environments. This report introduces a planning based collision avoidance methodology to generate collision-free trajectories for UAVs using sensor input including camera image and localization. The overall framework aims at tracking a reference trajectory and preventing collision to obstacles. In this report, the methodology for the planner module is introduced and the performance of the framework is demonstrated.

We are using Model Predictive Control(MPC) as the baseline for this problem. The MPC problem can be clarified in two parts: the objective function and the constraint functions. The objective function aims at minimizing the difference between execute trajectory and reference trajectory with minimum control cost. The constraint aims at limiting the maximum velocity and acceleration while keeping the safety distance to obstacles during navigation. By linearizing this MPC formulation and solving in terms of a Quadratic Programming (QP) problem, a trajectory that satisfies all the requirements will be generated in real-time.

In the experiment, we test the system in three different indoor and outdoor environments in simulation. The results show that MPC can achieve a success rate up to 90% in trajectory generation and collision avoidance, while the benchmark method can only achieve 40% success rate. In addition, experiments have been conducted for the computation time of the QP solver. The result shows that the planner could run up to 100Hz, which is 3 times faster than the SQP solver and completely satisfied the requirement to run in real-time.

In conclusion, we have introduced a  MPC planner based framework for dynamic navigation of UAVs in indoor environments. The system is proved to be able to avoid collisions and run stably in real-time.

More details can be found [here](https://www.youtube.com/watch?v=UeBShELDzyM).


<!-- This is an item in your portfolio. It can be have images or nice text. If you name the file .md, it will be parsed as markdown. If you name the file .html, it will be parsed as HTML.  -->
