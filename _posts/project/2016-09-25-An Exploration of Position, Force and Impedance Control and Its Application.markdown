---
layout: project
title:  "An Exploration of Position, Force and Impedance Control and Its Application"
date:   2016-09-25 16:54:46
categories:
- project
img: portfolio_01.jpg
carousel:
- portfolio_01.jpg
- proj01_1.jpg
- proj01_2.png
- proj01_3.png
- proj01_4.png
---
An Exploration of Position, Force and Impedance Control and Its Application
-----------------
The goal of this project is applying some control theories on the experiment setup which consists of two parts: Allegro Hand and Optoforce force sensors. Currently I only mounted the force sensor on the index finger as shown in the figure above and realized joint position, contact force and impedance control.

For the control method, the joint position control is already developed in ROS package from Wonik Robotics. In the contact force control, I design an experiment to let the finger apply contact force on a horizontal plane and supposed that there’s no motion when applying force. I first calculated the Jacobian Matrix of the finger and used the dynamics equation to solve the relation between the torque of joints and the contact force on the fingertip, ignoring the acceleration and velocity terms in the equation. By doing these the feedforward loop was completed. Then I used the force data from Optoforce as a feedback to calibrate the contact force by PI control. 

The figures below show the results of contact force control compared with the desired force changes. In these figures, X axis is time (second) and Y axis is force (Newton). We can see the errors clearly in the one-step force variation. The actual force spend about 0.15s to become stable, which is too slow for dynamic control experiments. Also the actual force change is slower than the desired change by about 0.025s. That is, in my point of view, the main cause of the poor performance of my force control, since it will influence the PID control I applied in the program. What's worse, it is sure that the delay is caused by hardware, so I can't do much to improve that. 

![proj01_2](/assets/img/project/carousel/proj01_2.jpg)

![proj01_3](/assets/img/project/carousel/proj01_3.jpg)

![proj01_4](/assets/img/project/carousel/proj01_4.jpg)

