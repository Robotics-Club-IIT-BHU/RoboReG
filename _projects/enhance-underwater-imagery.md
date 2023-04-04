---
title: Enhance UnderWater Imagery

description: |
  Takle the brightness of the images affected by factors such as refraction and absorption, suspended particles in the water, and color distortion results in a noisy and distorted visual data.

people:
  - viditagarwal 

layout: project
image: "/img/enhance-underwater-imagery/results.png"
last-updated: 2020-04-04
---
Autonomous underwater vehicles (AUVs) rely on a variety of sensors for decision-making, with vision-based sensors being one of the most appealing. Nevertheless, the visual data must be improved because red quickly fades and turns the photos blue, and the brightness of the photographs is also impacted by minute variations in the object's altitude above the seafloor. A noisy and distorted visual data is caused by variables including refraction and absorption, suspended particles in the water, and colour distortion.

First row consists of ground truth that we want, second row consists of visual data as seen underwater.

<p align="center">

   <img width="800" height="400" src="\img\enhance-underwater-imagery\visual-data.png">
   
</p>

To tackle this Pix2Pix GANs have been used to restore images. It's a Conditional Adversarial Network which performs image to image translation by translating an image from any arbitrary domain X to another arbitrary domain Y. By letting X be a set of distorted underwater images and Y be a set of undistorted underwater images, we can generate an image that is the enhanced version of the given underwater image.

1st column: Underwater Image / 2nd column: Ground Truth / 3rd column: Generated Image

<p align="center">

   <img width="600" height="200" src="\img\enhance-underwater-imagery\results.png">
   
</p>
<p align="center">

   <img width="600" height="200" src="\img\enhance-underwater-imagery\results1.png">
   
</p>
<p align="center">

   <img width="600" height="200" src="\img\enhance-underwater-imagery\results2.png">
   
</p>




