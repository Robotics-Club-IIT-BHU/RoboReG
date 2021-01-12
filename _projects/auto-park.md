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
image: "./img/auto-park/parking.gif"
last-updated: 2020-10-16
---

The primary aim of our project is to autonomously and smoothly park multiple cars at the same time without any sort of collisions between them. We aim to do this using the currently popular concept of Reinforcement Learning. The main reason we use this, in place of classical methods, is that we wish to see how the agent responds to stochasticity or randomness in the environment.

![Parking](./img/auto-park/full-parking.png)

We also use Image processing using a Convolutional Neural Network to automatically detect empty parking slots, and to gauge the location of the car and obstacles. We do not, however, directly use this to control the car. The car itself gets an alternative set of inputs.

We believe that such a system will be able to combine the benefits of the processing power of a machine and the intelligence of a human to deal with sticky situations.

We have built our environment in the form of an OpenAI gym in Pybullet.

![Racecar](./img/auto-park/racecar.png)

The agent(car) gets its inputs in the form of 14 readings, namely its position(x, y), velocity(x, y), orientation(x, y) and readings from 8 proximity sensors, each at angle of 45 degrees. We do not use the overhead camera images for training, even though they may eventually be better, as training on camera images is quite heavy.

![Surround Detection](./img/auto-park/surround-detection.png)

Through this project, we aim to visualize how an everyday task like parking a car, which is not exactly very simple, is done by an agent without any explicit understanding of how a car is parked.
