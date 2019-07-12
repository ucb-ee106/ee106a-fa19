---
layout: home
title: Home
nav_order: 0
description: >-
    Just the Class is a modern, highly customizable, responsive Jekyll theme
    for developing course websites.
---

# EE C106a/206a | Introduction to Robotics
{: .mb-2 }
Fall 2019
{: .mb-0 .fs-6 .text-grey-dk-000 }

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

An introduction to the kinematics, dynamics, and control of robot manipulators, robotic vision, and sensing. The course covers forward and inverse kinematics of serial chain manipulators, the manipulator Jacobian, force relations, dynamics, and control. It presents elementary principles on proximity, tactile, and force sensing, vision sensors, camera calibration, stereo construction, and motion detection. The course concludes with current applications of robotics in active perception, medical robotics, and other areas.
