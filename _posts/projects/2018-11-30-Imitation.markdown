---
layout: post
title: Human Imitation 
author: Sanghyun Kim
date:   2018-11-30 7:00:00 -0400
permalink: /Imitation-project
categories: projects
tags: HQP
excerpt: We implemented various algorithms to transfer from human motion to robot.  

image: /assets/img/project-images/7.imitation/main.png
imageAlt: HQP logo
image-slider: /assets/img/project-images/7.imitation/main.png

---
### Overview
This is my personal project in order to perform my motions in the humanoid robot. I implemented a few of algorithms using FABRIK, tensor algebra, and deep learning.

### Algorithms and Results
<div class="row projects-display">
	<div class="six columns">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/QzGgV9KHaZI" frameborder="0" allowfullscreen></iframe>
        </div>
	</div>
	<div class="six columns">
		<h5> Hand Motion and Force Mapping</h5>
		<li> Postural synergies based algorithm  </li>
		<li> See more <a href="{{site.url}}/robothand-project"> Robot Hand Project</a> </li>
	</div>
</div>
<div class="row projects-display">
	<div class="six columns">
		<h5> FABRIK based algorithm</h5>
		<li> We used Forward And Backward Reaching Inverse Kinematics (FABRIK) in order to calculate joint position.  </li>
		<li> To track my motion, I used VR device.</li>
		<li> See more <a href="{{site.url}}/UR2018"> UR2018</a> </li>
	</div>
	<div class="six columns">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/PfxoOjAHuBw" frameborder="0" allowfullscreen></iframe>
        </div>
	</div>
</div>
<div class="row projects-display">
	<div class="six columns">
		<div class="images">
			<img alt="Awesome Check In" height="100" src="{{ site.url }}/assets/img/project-images/7.imitation/rnn.png">
		</div>
	</div>
	<div class="six columns">
		<h5> Recurrent Neural Network based algorithm</h5>
		<li> We used Recurrent Neural Network in order to train the human motion.  </li>
		<li> We validated it in robotic simulator, V-REP. </li>
		<li> See more <a href="{{site.url}}/URAI2016"> URAI2016</a> </li> 
	</div>
</div>

