---
layout: home
title: Home
nav_order: 0
description: >-
    Course website for EE 106/206a Fall 2019
---
<div class="parallax-window" data-parallax="scroll" data-image-src="assets/background.png" data-speed="0.1">
# EE C106a/206a | Introduction to Robotics
{: .mb-2 }
Fall 2019
{: .mb-0 .fs-6 .text-grey-dk-200 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
<div class="role">
  {% for staffer in instructors %}
  {{ staffer }}
  {% endfor %}
</div>

{% if site.announcements %}
{{ site.announcements.last }}
<a href="{{ site.baseurl }}/announcements" class="btn btn-outline fs-3">
  All Announcements
</a>
{% endif %}

## Course Description

This course is an introduction to the field of robotics. It covers the fundamentals of kinematics, dynamics, and control of robot manipulators, robotic vision, and sensing. The course deals with forward and inverse kinematics of serial chain manipulators, the manipulator Jacobian, force relations, dynamics, and control. It presents elementary principles on proximity, tactile, and force sensing, vision sensors, camera calibration, stereo construction, and motion detection. The course concludes with current applications of robotics in active perception, medical robotics, autonomous vehicles, and other areas.

Students are expected to have a background in linear algebra, calculus, and basic physics, as well as familiarity with the Python programming language. The lectures are supplemented with homeworks and experimental work in the laboratory using two Baxter robots, and multiple mobile Turtlebot robots. There are two midterms, but no final exam. The last month is devoted to the design and implementation of a final project, carried out in groups of ~4 students.

The required text is Richard Murray, Zexiang Li and S. Shankar Sastry: "A Mathematical Introduction to Robotic Manipulation" (first edition digitally available <a href="http://www.cds.caltech.edu/~murray/mlswiki/?title=First_edition">here</a>). Additional lectures will cover the basics of computer vision, path planning, state estimation and control. 
</div>
