---
title: Waste Autonomous Robotics

description: |
  Providing Solutions for an Autonomous Waste Management System.

people:
  - antarabanerjee
  - atulkumar
  - aditiagarwal
  - niranthsai
  - lokeshkrishna
  
layout: project
image: "/img/auto-waste/design-vision-model.jpg"
last-updated: 2020-02-26
---

![working-model-design](/img/auto-waste/working-model-design.png)

Although still a major segment of our population relies on manual labour at dumpyards it cannot be denied that their lives are at a risk and they become prone to health hazards. Many autonomous solutions with implementation of robotics and artificial intelligence have already emerged in industries.

WHAT WE AIM TO DO
Taking an inspiration from the existent solutions we are trying to contribute in this field with an endeavour to provide solutions for waste management system.

WORK ACCOMPLISHED SO FAR
We are working on segregating 5 different types of plastic wastes for different recycling purposes. The 5 classes of plastics are- HDPE,LDPE,PVC,PET,Polystyrene.
We have created a vision system with Deep Learning. The training dataset has been created from scratch by us from different pictures of commonly used plastic objects.
The vision system works as a primary filter that groups different plastic objects into categories that the particular plastic object is likely to be made of. The
4 categories of the vision system are:-

1) LDPE and PET
![simu-ldpe-pet](/img/auto-waste/simu-ldpe-pet.jpg)
![real-ldpe-pet](/img/auto-waste/real-ldpe-pet.jpg)

2) Polystyrene
![simu-polystyrene](/img/auto-waste/simu-polystyrene.png)
![real-polystyrene](/img/auto-waste/real-polystyrene.jpg)

3) HDPE and PVC
![simu-hdpe-pvc](/img/auto-waste/simu-hdpe-pvc.png)
![real-hdpe-pvc](/img/auto-waste/real-hdpe-pvc.png)

4) HDPE,LDPE and PET
![simu-hdpe-pet-ldpe](/img/auto-waste/simu-hdpe-pet-ldpe.jpg)
![real-hdpe-pet-ldpe](/img/auto-waste/real-hdpe-pet-ldpe.jpg)

The vision model works both on real world object classification and simulated object classification. Transfer learning VGG 16 model has been used to improve accuracy of the vision system. The primary segregation based on vision system has been worked out on physics simulator Pybullet- a python module for physics simulations of robots, where a KUKA Robotic Arm has been used to pick and place the respective object into its category.

FUTURE WORK SCOPE
The vision system serves as a primary filter where plastic objects have been currently classified under more than 1 plastic type. To get accurate classification further haptic technology can be introduced along with the vision system to extract sensory parameters from the plastic objects and match them to their particular plastic type.
Compression tests that provide information regarding the material's compressive strength, yield strength, elastic limit and elastic modulus can be carried out along with the vision system , since each plastic type has its unique mechanical properties.
