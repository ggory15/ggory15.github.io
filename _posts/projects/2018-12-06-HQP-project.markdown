---
layout: post
title: Mobile Manipulation
author: Sanghyun Kim
date:   2018-12-06 7:00:00 -0400
permalink: /HQP-project
categories: projects
tags: HQP
excerpt: We are developing the controller of the dual-arm mobile manipulator by using HQP. In this study, we suggests the task transition algorithm to handle the discontinuity of the control input.

github: https://github.com/ggory15/HQP_DualArmMobile
#external-website: http://dyros.snu.ac.kr/project/non-holonomic-mobile-manipulator/

image: /assets/img/project-images/awesome-checkin/checkin2-screensaver.png
imageAlt: HQP logo
image-slider: /assets/img/project-images/slider-images/mobile_mani_slide.png

sliderData:
- video: "http://www.youtube.com/embed/-lfnLhmSk3M"
- video: "http://www.youtube.com/embed/K8RnMAA0rg4"
- video: "http://www.youtube.com/embed/4efccbsBLI4"
- video: "http://www.youtube.com/embed/JkTF-9RKoDM"

---
### Overview
Mobile robot and manipulator have a long history on their development. Combining these two robots, mobile manipulator has the potential of versatile skills. It has a high dimensional state space. However, combining these two robots causes many problems. First of all, the control system becomes complicated. Most manipulators actuate with the assumption that their basement is fixed. On the other hand, the mobile base and the manipulator give dynamic effects to each other. Therefore, we should consider the effects when we control the robot. Secondly, the target control accuracy would be lower than a fixed manipulator. As containing high dimensional state space, it inevitably leads to uncertainty (especially in mobile part).

To handle these problems, we are focusing on controlling and planning this mobile manipulator.

### Experimental Equipments
The robot consists of two robots. The mobile base is [**Clearpath Husky**](https://www.clearpathrobotics.com/husky-unmanned-ground-vehicle-robot/) and the manipulator is [**Franka Emika Panda**](https://www.franka.de/panda/).

It has a powerful computation unit to solve complicated whole-body dynamics and plan motions in high dimensional state space. The specification is described below.
+ CPU: Intel i7-7700K
+ RAM: 16 GB
+ Storage (SSD): 500 GB
+ OS: Ubuntu 16.04 (with preempt_rt kernel)

### Algorithms
+ Controller
	- Wholebody controller based on the HQP controller
	- Task transition algorithm for the HQP frameworks (with Joint limit, singularity, and obstacle avoidance algorithm)
+ Planner
	- Basic RRT(-connect) algorithm
	- VKC based dual-arm manipulation algorithm 

### Experimental Results

{% include flexslider_video.html %}

We developed the controller for nonholonomic mobile manipulator using the HQP framework. In addition, we developed a novel approach to generate continuous control input during task transition. These videos show the proposed algorithm can be applied at various scenarios.

