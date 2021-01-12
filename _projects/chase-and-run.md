---
title: Chase and Run

description: |
  Developing a fast and robust control system for dynamic games aimed at identifying Nash equilibrium strategies and emergent behaviour in competitive settings. 

people:
  - ayushshaw
  - raghavsoni
  - yashsahij
  - niranthsai
  - lokeshkrishna

layout: project
image: "./img/chase-and-run/cars.gif"
last-updated: 2020-03-04
---

One of the key challenges and active areas of research in robotics and control systems are multi-agent systems, especially those which involve collaboration or competition between individual systems. The traditional control strategies in these situations require a lot of control equations with underlying mathematics and physical dynamics of the system along with the communication protocols. This however, confines these systems to work in an already known fashion without display of any new behaviour. Through this project, we aim to visualize new emergent behaviours in competitive as well as mixed settings (competitive + collaborative) using multi-agent reinforcement learning as they provide a more robust and efficient way of developing a control system with the ability to perform new behaviours than traditional methods.

Adversarial Chase and Run Cars Gym is a gym environment, to test and develop algorithms related to Multi Agent Systems, especially those related to Multi-Agent Reinforcement Learning. This was done under the Robotics Research Group (RoboReG) to try and learn emergent behavior between agents competing against each other via Reinforcement learning and how it could generate new control strategies.

This gym environment consists of 2 mobile robots, where the task of one of the robots is to chase the other one, while the other simply avoids the chaser. The environment also consists of walls which define the operating area, so that the robots remain confined in a particular area. Though this has been done in 2D-worlds, analyzing emergent behaviour in a physical world with real physics and dynamics is a relatively less explored area.

![Cars]({{ site.base }}/img/chase-and-run/auto.png)

The gym environment was built in the physics simulator PyBullet - a python module for physics simulations of robots, because of its easy usage and integration with RL frameworks like Stable Baselines. Work is currently being done on training the agents to compete via Multi Agent Reinforcement Learning.

The mobile robots that are being used in the environment were built and designed completely in Blender, and were exported as URDFs, so that they could be imported in all physics simulators.
