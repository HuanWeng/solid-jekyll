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
This project is an academic project. In this project I designed, fabricated, and programmed a mobile robot made of laser cut and 3D printed parts, which follows a Mario Kart circuit – for Northwestern’s Tech Cup 2016.

This robot can be devided into three parts: a android phone with its camera used to sense the line ahead, a PCB used to receive the data from the phone and send the PWM signals to the motor, and the vehicle to hold all the these parts.

While the robtot running on the map, the camera sense the area ahead the vehicle and identify the location of the line by check the RGB value from the screen of the camera. This information will be sent to PCB using serial communication and based on this, the PIC32 on that board executes differential control to the wheel speed of the vehiles, which is driven by two motors.

Finally I get the first place in the competition, using 29 seconds to complete the circuit, while the average of the competiors is about 45 seconds. 
