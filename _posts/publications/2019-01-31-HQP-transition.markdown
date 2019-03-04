---
published: true
layout: post
title: Continuous Task Transition Approach for Robot Controller based on Hierarchical Quadratic Programming
author: Sanghyun Kim, K. Jang, S. Park, Y. Lee, S. Lee, and J.Park
name: IEEE Roboticis and Automation Letters
state: accepted
year: 2019
vol: 4
pp: 1603-1610
issue: 2
type: International_journal
date:   2019-01-31 7:00:00 -0400
permalink: /HQP-transition
categories: publications
tags: HQP, Task_Transition, Mobile Manipulator
excerpt: This article has been accepted in RA-L with ICRA 2019. See you soon.
github: https://github.com/ggory15/HQP_DualArmMobile

pdf: http://dyros.snu.ac.kr/wp-content/uploads/2019/01/revision.pdf
sourcecode: 

image: /assets/img/post-images/slider-images/HQP_icra.png
imageAlt: HQP logo
image-slider: /assets/img/post-images/slider-images/HQP_icra.png

sliderData:
- video: "https://www.youtube.com/embed/atcX-sf4098"
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
[**PDF file**](http://dyros.snu.ac.kr/wp-content/uploads/2019/01/revision.pdf)

### Source Codes
You can see the source codes in my [**git repository**](https://github.com/ggory15/HQP_DualArmMobile).
The source codes will be operated in Windows 10, ubuntu 16.04, and 14.04

### Multimedias
<div class="row projects-display">
    <div class="twelve columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/-lfnLhmSk3M" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>

### See More
Please Visit [**HQP project**]({{ site.url}}/HQP-project) and [**Task Transition project**]({{ site.url}}/tasktransition-project).


