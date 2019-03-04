---
layout: post
title: Mobile Manipulation using HQP
author: Sanghyun Kim
date:   2018-12-06 7:00:00 -0400
permalink: /HQP-project
categories: projects
tags: HQP, mobile-robot
excerpt: We are developing the controller of the dual-arm mobile manipulator by using HQP. In this study, we suggests the task transition algorithm to handle the discontinuity of the control input.

github: https://github.com/ggory15/HQP_DualArmMobile
external-website: http://dyros.snu.ac.kr/project/non-holonomic-mobile-manipulator/

image: /assets/img/project-images/1.mobile/mobile.jpg
imageAlt: HQP logo
image-slider: /assets/img/project-images/1.mobile/mobile.jpg

---
### Overview
Mobile robot and manipulator have a long history on their development. Combining these two robots, mobile manipulator has the potential of versatile skills. It has a high dimensional state space. However, combining these two robots causes many problems. First of all, the control system becomes complicated. Most manipulators actuate with the assumption that their basement is fixed. On the other hand, the mobile base and the manipulator give dynamic effects to each other. Therefore, we should consider the effects when we control the robot. Secondly, the target control accuracy would be lower than a fixed manipulator. As containing high dimensional state space, it inevitably leads to uncertainty (especially in mobile part).

To handle these problems, we are focusing on controlling and planning this mobile manipulator.

### Experimental Equipments
The system consists of two robots. The mobile base is [**Clearpath Husky**](https://www.clearpathrobotics.com/husky-unmanned-ground-vehicle-robot/) and the manipulator is [**Franka Emika Panda**](https://www.franka.de/panda/).

It has a powerful computation unit to solve complicated whole-body dynamics and plan motions in high dimensional state space. The specification is described below.
+ CPU: Intel i7-7700K
+ RAM: 16 GB
+ Storage (SSD): 500 GB
+ OS: Ubuntu 16.04 (with preempt_rt kernel)

### Algorithms
<div class="row projects-display">
    <div class="six columns">
        <div class="images">
            <img alt="JUCE" src="{{ site.url }}/assets/img/project-images/1.mobile/nonholo.png">
        </div>
     </div>
    <div class="six columns">
        <div class="images">
            <img alt="JUCE" src="{{ site.url }}/assets/img/project-images/1.mobile/overview.png">
        </div>
    </div>
</div>
+ Controller
	- Wholebody controller based on the HQP controller.
	- Task transition algorithm for the HQP frameworks (with Joint limit, singularity, and obstacle avoidance algorithm) 
	- Momentum based observer

+ Planner
	- Basic BiRRT(-connect) algorithm
	- VKC based dual-arm manipulation algorithm 

### Experimental Results
<div class="row projects-display">
    <div class="six columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/FyiSZ1lomSs" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>

    <div class="six columns">
        <h5> Task Transition Algorithm </h5>
        <li> See also <a href="{{ site.url}}/tasktransition-project"> Transition Project </a> </li>
        <li> See also <a href="{{site.url}}/mobile-project"> Related Papers </a> </li>
        </div>
</div>

<div class="row projects-display">
    <div class="six columns">
        <h5> Coffee Delivery Demo #1 </h5>
        <li> Making trajectory by using BiRRT </li>
        <li> Controlling by Whole-body HQP controller </li>
        <li> Task Transition by considering multiple tasks </li>
        </div>

    <div class="six columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/K8RnMAA0rg4" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>
<div class="row projects-display">
    <div class="six columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/4efccbsBLI4" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>

    <div class="six columns">
        <h5> Coffee Delivery Demo #2 </h5>
        <li> Making trajectory by using BiRRT </li>
        <li> Controlling by Whole-body HQP controller </li>
        <li> Task Transition by considering multiple tasks </li>
        </div>
</div>
<div class="row projects-display">
    <div class="six columns">
        <h5> Momentum Observer Demo </h5>
        <li> Detecting disturbances using momentum based observer </li>
        <li> Compliance Control </li>
        </div>
        
    <div class="six columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/JkTF-9RKoDM" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>



### TODO
+ Dual Arm Manipulation
	- Although it is already done in simulation, we cannot experiments with the real robot. We want to buy one more manipulator! (Give me the money.)
<div class="row projects-display">
    <div class="four columns">
        <div class="images">
            <img alt="JUCE" src="{{ site.url }}/assets/img/project-images/1.mobile/dualarm.png">
        </div>
     </div>
    <div class="six columns">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/UERT8sQRnBc" frameborder="0" allowfullscreen></iframe>
        </div>
     </div>
</div>


+ More powerful planner 
	- (DDP? )
+ Door openning algorithm
