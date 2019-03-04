---
published: true
layout: post
title: Whole-body control for nonholonomic mobile manipulator using Hierarchical Quadratic Programming and Continuous Task Tranasition
author: Sanghyun Kim, K. Jang, S. Park, Y. Lee, S. Lee, and J. Park
name: IEEE Interantional Conference on Advanced Robotics & Mechatronics
state: under-review
year: 2019
# vol: 4
# pp: 1603-1610
# issue: 2
type: International_conference
date:   2019-02-22 7:00:00 -0400
permalink: /mobile-project
categories: publications
tags: HQP, mobile
excerpt: This article has been summited on ARM 2019
#github: https://github.com/ggory15/HQP_DualArmMobile

#pdf: http://dyros.snu.ac.kr/wp-content/uploads/2019/01/revision.pdf
sourcecode: 

image: /assets/img/post-images/slider-images/arm.png
imageAlt: HQP logo
image-slider: /assets/img/post-images/slider-images/arm.png

pdf: #http://dyros.snu.ac.kr/wp-content/uploads/2018/07/IK_shortver-1.pdf
sourcecode: 
---

### Abstact 
This paper presents a real-time self-collision
avoidance algorithm for a differentially driven mobile manip-
ulator. When the manipulator and the mobile base are close
to each other, attractive force is exerted on the mobile base
for the manipulator to come close to the collision-free area
in the workspace of the manipulator. The force is always
generated even if the manipulator approaches the mobile base
in any direction. In this respect, the proposed algorithm has a
distinct advantage over existing methods which focus on simply
pushing the links away from each other and do not consider
the mobile base with non-holonomic constraints. The force and
the resulting torque are converted to the desired accelerations
of the mobile base and they construct the avoidance task. The
task is smoothly inserted with a top priority to the controller
based on hierarchical quadratic programming. The proposed
algorithm was implemented on the differentially driven mobile
base with the 7-DoFs robotic arm, and its performance was
demonstrated during various experimental scenarios.

### PDF 
<!-- [**PDF file**](http://dyros.snu.ac.kr/wp-content/uploads/2019/01/revision.pdf) -->
PDF will be uploaded after acceptance on the conference.

### Multimedias
<div class="row projects-display">
    <div class="twelve columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/FyiSZ1lomSs" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>

### See More
Please Visit [**HQP project**]({{ site.url}}/HQP-project) and [**IROS 2019**]({{ site.url}}/IROS2019) for the self-collision avoidance algorithm.
