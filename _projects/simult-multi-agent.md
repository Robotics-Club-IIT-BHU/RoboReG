---
title: Simultaneous Multitasking Agent

# notitle: true

description: |
  Training a Robot for doing multiple tasks simultaneously like a human being, using one image frame.

people:
  - amanmishra
  - akshatsood
  - adityakumar
  - mainaksamanta
  - niranthsai
  - lokeshkrishna

layout: project
image: "/img/simult-multi-agent/env.png"
last-updated: 2018-08-06
---

Doing multiple tasks simultaneously is generally a human behaviour. But is it possible for a robot? In that part our project is based on. We are trying to explore how a robot can do multiple tasks which have low correlation between them simultaneously using a image frame and its depth value.

![Baxter Description]({{ site.base }}/img/simult-multi-agent/baxter_desc.png)
![Baxter Working]({{ site.base }}/img/simult-multi-agent/baxter.gif)
![Baxter pic]({{ site.base }}/img/simult-multi-agent/baxter.png)

We first divided our project into some Tasks:
Task-1: Make the environment and experimental setup
Task-2: Find Joint Reward function.
Task-3: Learn easy simultaneous tasks.
Task-4: Increase Task complexity.
Task-5: Increase interaction complexity.

For our project we have made a Pybullet gym environment. We have used a prebuilt agent Baxter(Two handed robot).

For state the environment returns us a dictionary containing-

1. Eye view image
2. Corresponding depth map
3. Hand end effectors position with respect to the agent

![Image Data]({{ site.base }}/img/simult-multi-agent/image_data.png)
![Depth Data]({{ site.base }}/img/simult-multi-agent/depth_data.png)

For actions the environment uses a Bezier curve (trajectories through some fixed points) function.
For making a trajectory everytime we find the current end effector centroid, box centroid and their mid point as the fixed points of the curve and then using the input weights we made trajectories for both the hands.

For each trajectory we have taken points on it at 5 different timesteps and moved the hand to the points.
One step is considered as traversing one trajectory in this environment.

Reward:
For the whole trajectory we counted the cumulative reward by discounting the cumulative reward of previous time step.
