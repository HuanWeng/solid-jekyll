---
layout: project
title:  "Android Line Follower Mobile Robot"
date:   2016-06-15 16:54:46
categories:
- project
img: portfolio_03.jpg
carousel:
- portfolio_03.jpg
- proj03_1.jpg
- proj03_2.jpg
- proj03_3.jpg
- proj03_4.jpg
---
Android Line Follower Mobile Robot
-----------------
The goal of this project is applying some control theories on the experiment setup which consists of two parts: Allegro Hand and Optoforce force sensors. Currently I only mounted the force sensor on the index finger as shown in the figure above and realized joint position, contact force and impedance control.

For the control method, the joint position control is already developed in ROS package from Wonik Robotics. In the contact force control, I design an experiment to let the finger apply contact force on a horizontal plane and supposed that there’s no motion when applying force. I first calculated the Jacobian Matrix of the finger and used the dynamics equation to solve the relation between the torque of joints and the contact force on the fingertip, ignoring the acceleration and velocity terms in the equation. By doing these the feedforward loop was completed. Then I used the force data from Optoforce as a feedback to calibrate the contact force by PI control. The figures below show the results of contact force control.

For the impedance control, currently I simplified the model by ignoring the mass and damper properties of the finger. So the whole finger was supposed to be like a virtual spring, as shown below, once setting the stiffness and the original position of the fingertip in 3 directions. This work is applied in other research experiments in my lab.
