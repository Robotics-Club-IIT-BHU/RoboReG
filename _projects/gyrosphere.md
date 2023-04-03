---
title: Gyrosphere - The Spherical Bot

description: A ball-shaped mobile robot with spherical external shape typically made of a spherical shell serving as the body of the robot and an internal driving unit (IDU) that enables the robot to move.

people:
  - astitvagupta
  - sanidhyataparia
  - navalselvan

layout: project
image: "/img/gyro/gyrosphere.gif"
last-updated: 2023-04-04
---

## Introduction:

Gyrosphere is a ball-shaped mobile robot with spherical external shape typically made of a spherical shell serving as the body of the robot and an internal driving unit (IDU) that enables the robot to move. Gyrosphere typically moves by rolling over surfaces. The rolling motion is commonly performed by changing the robot's center of mass (i.e., pendulum-driven system).

## Model of Gyrosphere

The Sphere model consists of an Internal driving unit (IDU) enclosed by two hemispherical shells joined together. The IDU is a tetrahedral skeleton made by joining four cylindrical rods connecting them tetrahedrally. End of the rods are attached with omni wheels which are in contact with the internal surface of the spherical unit except the top rod which has a ball and socket joint for maintaining the upright position of the IDU. Omniwheels used are controlled by BLDC motors. The central mass is attached below the driving unit.

<p align="center">

   <img width="350" height="280" src="https://robotics-club-iit-bhu.github.io/RoboReG/img/gyro/gyro_matplotlib-model.png">
   <img width="350" height="280" src="https://robotics-club-iit-bhu.github.io/RoboReG/img/gyro/gyro_pybullet_model.png">
</p>

## Results

### Achieved Objectives

#### A fully functional urdf file for our imporvised mechanism.

The designed urdf file is completely ready and can be used for Simulation in pybullet or in any other simulation software with a few tweaks.

1. Simulation with the Internal driving unit fixed

<p align="center">
<iframe width="560" height="315" src="https://user-images.githubusercontent.com/75927242/152683211-b4be53bd-7ec0-4552-bbc6-cfe37ffccaf4.mp4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

2. Simulaltion with the bot free, WITHOUT any proper controller. The work is in progress for it.

<p align="center">
<iframe width="560" height="315" src="https://user-images.githubusercontent.com/75927242/152683170-45838170-e293-4642-afdc-fee81c785365.mp4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

#### Linear Qudratic Regulator for accurate path following

We Have designed two controllers for Path following using LQR control.

1. Path following using the current position as the state vector. Video is attached below. Herethe controller was told to follow a sine curve At the end it can be observed that it traces the desired path upto high accuracy.
2. Path following using the current velocity as the state vector. Needs a bit more work.

<b>Curve Following using position in 3D space as state</b>

<p align="center">
<iframe width="560" height="315" src="https://user-images.githubusercontent.com/75927242/152682768-76f656b1-9296-49bc-9216-b5136866597f.mp4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

### Project Collaborators

- [Astitva Gupta](https://www.linkedin.com/in/astitva-gupta-26798312b)
- [Sanidhya Taparia](https://sanidhya-portfolio.vercel.app)
- [Naval Selvan. S](https://linkedin.com/in/naval-selvan-s-28620a201)
