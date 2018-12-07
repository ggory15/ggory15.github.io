---
layout: post
title: Robot Hand Control
author: Sanghyun Kim
date:   2018-12-04 7:00:00 -0400
permalink: /robothand-project
categories: projects
tags: HQP
excerpt: In this project, I want to figure out how to imitate human hand motion and force for the robot hand. 

github: https://github.com/ggory15/HQP_DualArmMobile
external-website: http://dyros.snu.ac.kr/project/non-holonomic-mobile-manipulator/

image: /assets/img/project-images/3.hand/hand.png
imageAlt: HQP logo
image-slider: /assets/img/project-images/3.hand/hand.png

---
### Overview
A robot hand can provide a great deal of manipulation capability to its user in a
tele-manipulation system. The method of controlling the robot hand with human
hand motion is one of the most important parts of such a system, as a human
hand can perform many types of operations given its number of joints, whereas
a robot hand is limited in terms of motion compared to that of human hand
motion. Thus, the functionality and controllability of dexterous robot hands
have been investigated in an effort to overcome the difficulty stemming from the
kinematic dissimilarity between robot and human hands.

To handle this problem, we developed the algorithm for tele-operation with tensor algebra. First, we proposed the algorithm for extracting postural synergies which can account for not only grasping motions but also individual characteristics. Second, we studied the algorithm for predicting the grasping force of the human using sEMG. 

### Experimental Equipments
We used the full-actuacted robot hand, [**Allegro Hand**](http://wiki.wonikrobotics.com/AllegroHandWiki/index.php/Allegro_Hand).
The specification of this robot is as follow.

<div class="row projects-display">
	<div class="six columns">
		<div class="images">
			<img alt="Awesome Check In" height="100" src="{{ site.url }}/assets/img/project-images/3.hand/allegro.png">
		</div>
	</div>
	<div class="six columns">
		<h5> Allegro Hand</h5>
		<li> 16-DoFs torque controlled robot </li>
		<li> Each finger has 4actuactors</li>
		<li> CAN protocole in Ubuntu 14.04/16.04, Windows </li>
	</div>
</div>
<div class="row projects-display">
	<div class="six columns">
		<h5> Motion Capture Studio</h5>
		<li> 24 Stereo Cameras with Vicon </li>
		<li> <a href="https://www.delsys.com/products/wireless-emg/"> sEMG Device </a> </li>
		<li> TCP/IP system </li>
	</div>
	<div class="six columns">
		<div class="images">
			<img alt="Awesome Check In" height="100" src="{{ site.url }}/assets/img/project-images/3.hand/motion1.png">
		</div>
	</div>
</div>

### Algorithms
+ Synergies Level Controller 
	- We proposed the controller for imitation human motions using synergies.
	- The proposed method uses a tensor to represent a multi-factor model relevant to different individuals and motions in multiple dimensions.
    - The effectiveness of the proposed new mapping algorithm is verified through experiments, which demonstrate better representation of hand motions with synergies and greater performance on grasping tasks than those of conventional synergy-based algorithms.
	- See also [**ISER2014**]({{ site.url}}/ISER2014)

+ Grasping Force Prediction
	- We proposed the grasping force prediction algorithm with tensor algebra.
	- Our algorithm can estimate the grasping force with various arm postures. To the best of our knowledge, this is first algorithm to handle the grasping force prediction with various arm postures.
	- See also [**JBEN2018**]({{ site.url}}//EMG-Force)

### Why we used Tensor?
+ Efficient data reduction algorithm
	- Singular Vector Decomposition (SVD) which is a matrix factorization is good data reduction algorithm.
	- Similarly, in the tensor space, the Tucker decomposition can decompose a nth order tensor. Therefore, it is easy to reconstruct the space with feature vectors.
	- Below figure is overview of our prediction algorithm using Tucker decomposition.
		<div class="images">
			<img alt="JUCE" src="{{ site.url }}/assets/img/project-images/3.hand/emg_overview.png">
		</div>

### Experimental Results
<div class="row projects-display">
    <div class="six columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/QzGgV9KHaZI" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
    <div class="six columns">
        <h5> Motion and Force Mapping </h5>
        <li> As you can see, we validated the proposed algorithm with various experiments. </li>
		<li> We used the motion capture studio to track human hand motions. </li>
		<li> Also, we used the wireless sEMG system, as metioned above. </li>		
	</div>
</div>

<div class="row projects-display">
	<div class="six columns">
		<h5> Grasping Force Prediction Test </h5>
		<li> Our algorithm can predict grasping forces. </li>
		<li> As you can see, the result is more accurate than <a href=""> the reference algorithm. </a> </li>
	</div>
	<div class="six columns images">
		<div class="flexslider">
			<ul class="slides">
	  			<li>
					<div class="images">
						<img alt="JUCE" src="{{ site.url }}/assets/img/project-images/3.hand/proposed_result.png">
					</div>
				</li>
				<li>  
					<div class="images">
						<img alt="JUCE" src="{{ site.url }}/assets/img/project-images/3.hand/modi_result.png">
					</div>
				</li>  
				<li>  
					<div class="images">
						<img alt="JUCE" src="{{ site.url }}/assets/img/project-images/3.hand/result22.png">
					</div>
				</li>  
			</ul>
		</div>
	</div>
</div>