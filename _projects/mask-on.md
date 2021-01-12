---
title: Mask-On

description: |
  This project includes using robots for human surveillance in shopping malls and grocery stores.

people:
  - jatineaga
  - payalpote
  - ananyasingh
  - vishwaschepuri
  - niranthsai
  - lokeshkrishna

layout: project
image: "/img/mask-on/mask-tracking.gif"
last-updated: 2019-08-06
---

The CORONA virus has taught us many things, right from sanitation of the body to surroundings. So this helps us to find out and keep the area virus free.

![Mall]("./img/mask-on/mall.jpg")

![Humans](./img/mask-on/diff_humans.jpg)

We are working on building two sets of pipelines while one at entrance and other on a turtle bot trying to find someone is not following protocols.

ENTRANCE - Facial mask detection along with body temperature checking.

TURTLE-BOT - This is a small bot which roams in the mall and tracks every person who comes into the camera feed and checks for a mask but if he fails to have it in the proper position then it will notify the mall's or store's authority to take action against the person involved in this.
![Bot](./img/mask-on/bot.png)

To make this happen, we started training and simulating a mall / grocery like environment using ros in the gazebo simulator. The turtle bot is used especially for getting precise information regarding any kind of activities such as cough and sneeze. We can also work on surveillance camera feed to find if any person is violating the protocols.

![Mask Detection](./img/mask-on/mask-detection.gif)

This project would help us become more precautious regarding masks and personal care i.e sanitation.
