---
layout: project
title:  "DC Motor Control with PIC32 and Matlab"
date:   2016-03-23 16:54:46
categories:
- project
img: portfolio_04.png
carousel:
- portfolio_04.png
- proj04_1.png
- proj04_2.jpg
- proj04_3.jpg
---
DC Motor Control with PIC32 and Matlab
-----------------
This is an academic project. The final project is to control the motion of a motor using Matlab based on the trajectories designed. 

I developed program to control the motor using PWM from PIC32, with current/torque and motion control loops using PID control.Also I realized serial communication between Matlab (client) and PIC32 (server) and plotted the trajectory results.

The figures below show the results of the motion of motor following a step trajectory and a smooth curve trajectory. We can conclude that the performance when following the curve is much better than that following the step trajectory. I think the reason is that the motor and encoder we use is not that precise. So when the trajectory includes some steps the error will be exaggerated and if there is no sudden changes in the trajectory, the motor will follow it better.

![proj04_2](/assets/img/project/carousel/proj04_2.jpg)

![proj04_3](/assets/img/project/carousel/proj04_3.jpg)
