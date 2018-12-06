---
published: true
layout: post
title: Continuous Task Transition Approach for Robot Controller based on Hierarchical Quadratic Programming
author: S. Kim, K. Jang, S. Park, Y. Lee, S. Lee, and J.Park
name: IEEE Roboticis and Automation Letters
state: (Revised and Resummit)
year: 2018
type: International_journal
date:   2018-09-05 7:00:00 -0400
permalink: /HQP-transition
categories: publications
tags: HQP
excerpt: This article is summitted in RAL and ICRA 2019. The state is 'revision and resummit'
github: https://github.com/ggory15/HQP_DualArmMobile

image: /assets/img/post-images/slider-images/HQP_icra.png
imageAlt: HQP logo
image-slider: /assets/img/post-images/slider-images/HQP_icra.png

sliderData:
- video: "http://www.youtube.com/embed/-lfnLhmSk3M"
---

### Abstact 
The robots with high Degrees of Freedom (DoF) such as humanoids and 
mobile manipulators are expected to perform multiple tasks
simultaneously. Hierarchical Quadratic Programming (HQP) can
effectively compute a solution for strictly prioritized tasks. However,
the continuity of control input is not guaranteed when the priorities
of the tasks are modified during operation. This paper proposes a
continuous task transition method for HQP based controller to insert,
remove, and swap arbitrary tasks without discontinuity. Smooth task
transition is assured because our approach uses activation parameters
of the new and existing tasks without modifying control structure.The
proposed approach is applied to various task transition scenarios
including joint limit, singularity, and obstacle avoidance to guarantee
the stable execution of the robot. The proposed  control  scheme  was 
implemented  on  a 7-DoF robotic arm, and its performance was
demonstrated by the continuity of control input during various task
transition scenarios.

### PDF 
If this paper is accepted, I will upload the pdf file.

### Source Codes
You can see the source codes in my [**git repository**](github: https://github.com/ggory15/HQP_DualArmMobile).
The source codes will be operated in Windows 10, ubuntu 16.04, and 14.04

### Multimedias
Videos may be not represented in mobile. Please, visit this website in PC, if you want to see these videos. 

<iframe width="960" height="540" src="https://www.youtube.com/embed/H69kzO3Obdk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> 

### See More
Please Visit [**HQP-project**]({{ site.url}}/HQP-project).


