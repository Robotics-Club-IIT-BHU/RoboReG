---
title: 3D-Occupancy-Maps-With-Quadrotors

description: |
  Simulated Hector Quadrotor In Gazebo and Mapped a Unknown environment.

people:
  - pratikmishra
  - chahakjethani
  - amiteshvatsa 

layout: project
image: "/img/3D-occupancy-maps/3D-map.png"
last-updated: 2023-04-04
---
You can map any world using this project. Just replace the new_world in 3D-Occupancy-Maps-With-Quadrotors/drone_test/worlds and rename it new_world.
You can create the occupancy map of your gazebo world.

Project Comprises of -

Our Package : We created a ROS package with necessary dependencies. This package serves the purpose of linking Hector Quadrotor and Octomap with appropriate remapping of topics. We start our drone with this package.

Hector Quadrotor : We chose to simulate our project using the Hector Quadrotor due to its huge functionality. This drone is equipped with a depth camera and kinect. Moreover, it's extremely popular and used across various projects.

Octomap : The point cloud data published is not always accurate and there are variances. The OctoMap package estimates the inaccuracies and  corrects them by establishing continuity in the probability function.

How Everything Links Are Shown Below

<p align="center">

   <img width="400" height="600" src="/img/3D-occupancy-maps/Connection.png">
   
</p>

base_link connects to base_stabilized from the above diagram and Tree is Completed.

<p align="center">

   <img width="600" height="400" src="/img/3D-occupancy-maps/base-link.png">
   
</p>
<p align="center">

   <img width="800" height="400" src="/img/3D-occupancy-maps/map.png">
   
</p>
