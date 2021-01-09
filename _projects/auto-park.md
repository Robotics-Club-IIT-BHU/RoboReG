---
title: Autonomous Parking

description: |
  Autonomous Parking Management through Multi-Agent Reinforcement Learning

people:
  - ajasragupta
  - vikhyathvenkatraman
  - amarjeetkeshri
  - princegond
  - niranthsai
  - lokeshkrishna

layout: project
image: "/img/auto-park/full-parking.png"
last-updated: 2020-10-16
---

The primary aim of our project is to autonomously and smoothly park multiple cars at the same time without any sort of collisions between them. We aim to do this using the currently popular concept of Reinforcement Learning. The main reason we use this, in place of classical methods, is that we wish to see how the agent responds to stochasticity or randomness in the environment.

![Parking](/img/auto-park/parking.png)

We also use Image processing using a Convolutional Neural Network to automatically detect empty parking slots, and to gauge the location of the car and obstacles.

We believe that such a system will be able to combine the benefits of the processing power of a machine and the intelligence of a human to deal with sticky situations.

We have built our environment in the form of an OpenAI gym in Pybullet.

![Racecar](/img/auto-park/racecar.png)

![Surround Detection](/img/auto-park/surround-detection.png)

Through this project, we aim to visualize how an everyday task like parking a car, which is not exactly very simple, is done by an agent without any explicit understanding of how a car is parked.
