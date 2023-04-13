---
title: Multipurpose Household Bot

description: |
  A multi-purpose household bot with a lot of innovative features with a limited hardware which solve small day to day problems.

people:
  - harshmahesheka
  - tusharsarkar
  - jaynilsheth 
  - pratyushsingh  

layout: project
image: "/img/household-bot/household-bot.gif"
last-updated: 2023-04-04
---

The fundamental concept behind this bot is to build a multifunctional home automation system with a tonne of features that make it affordable for the ordinary household. The majority of household bots available now only perform specific tasks, such as cleaning or playing, but we can add more functionalities without considerably increasing hardware (which won't increase the cost). The bot will assist with all daily tasks, including child care, cleaning, security, and many other things. Its usability will rise and the price will drop thanks to numerous simple and creative innovations like DIY guides and detachable parts. Also, we'll make it programmable and customizable by users so they can play around with it, learn from it, and add new features.

With SolidWork, we created our own vacuum-cleaning home robot from scratch and tested it using techniques like stress analysis and airflow modelling to ensure that it would work in practise.


<p align="center">

   <img width="600" height="400" src="/img/household-bot/velocity-flow.png">
   
</p>

<p align="center">

   <img width="600" height="400" src="/img/household-bot/pressure-flow.png">
   
</p>

We implemented three algorithms for Autonomus Mapping, Autonomus Navigation, and Autonomus Optimal Full Coverage while using differential drive and the ROS Navigation stack for navigation. Also, we used the YoloV3 and Resnet algorithms for baby monitoring. Facial recognition and threat detection.

<p align="center">

   <img width="600" height="400" src="/img/household-bot/navigation.png">
   
</p>

We use a custom build AI model, combining both, a pretrained ResNet model and the OpenCV haarcascade funtion to develop face recognition algorithm. 

Bot follows the baby around and triggers an alarm or sends parents a message when the baby is near a harmful object or so. Here we use custum build algorithm using pretrained YOLOv3 weights to perform object detection.
The YOLOv3 (You Only Look Once) model is an object detection architecture that uses a 106 layer network comprising of multiple Convolution, residual and 1*1 kernel layers to perform the object detection task.

<p align="center">

   <img width="600" height="400" src="/img/household-bot/baby-following.png">
   
</p>

Our bot is just what a working mom needs for their child, from cleaning the house to taking care of their infant by watching and following it. Using our bot, you may even make video calls from any distant location! With our bot, which is truly versatile, we have you covered in terms of communication, security, hygiene, and child's social development.
