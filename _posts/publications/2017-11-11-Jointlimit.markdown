---
published: true
layout: post
title: Joint limit avoidance of non-holonomic mobile manipulator using weighting matrix in generalized pseudo-inverse 
author: K. Jang, Sanghyun Kim, S. Park, and J.Park
name: 한국정밀공학회 2017년도 추계학술대회논문집
state: accepted
year: 2017
type: Domestic_conference
date:   2017-11-11 7:00:00 -0400
permalink: /jointlimit
categories: publications
tags: Task_Transition
excerpt: This article is accepted in 한국정밀공학회 2017년도 추계학술대회논문집.

image: /assets/img/post-images/slider-images/NO.jpg
imageAlt: HQP logo
image-slider: /assets/img/post-images/slider-images/NO.jpg

pdf: 
sourcecode: 

---

### Abstract
모바일 매니퓰레이터는 매니퓰레이터와 바퀴나 다리가 달린 이동 로봇이 결합된 로봇으로 매니퓰레이터가 가진 조작성과 이동 로봇이 가진 이동성을 동시에 가지고 있다. 이러한 장점으로 모바일 매니퓰레이터는 기존의 목표 위치 경로를 추종하는 작업에 필요한 자유도 이외에 여유자유도를 활용하여 로봇의 제한 조건을 회피하면서 작업을 수행할 수 있다. 따라서 본 논문에서는 여유자유도를 활용하여 매니퓰레이터의 관절 제한을 회피하면서 목표 경로를 추종하는 관절의 움직임을 생성하여 제어하였다. 관절 속도는 가중 행렬을 반영한 모바일 매니퓰레이터 전체 자코비안 행렬의 의사 역행렬을 통해 구하였다. 가중 행렬을 구성하기 위해 매니퓰레이터 각 관절의 상한치, 하한치와 현재 관절 값을 반영한 전위 함수를 도입하였고, 관절 값 변화에 따른 전위 함수의 구배(gradient) 값을 통해 가중 행렬에 가중치를 대입하였다. 관절 제한 회피에 대한 검증은 시뮬레이션 환경에서 비홀로노믹(non-holonomic) 특성을 가진 모바일 매니퓰레이터의 관절 값을 확인하여 실시하였다. 

### See More
Please visit [**Task Transition project**]({{ site.url}}/tasktransition-project).