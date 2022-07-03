# Automated 3d printed robot arm for Pick & Place
This project is an applying of deep learning to robot arm for done some repetitive task. Fortunately, there is an Very cool! opensource 3d pritned robot arm and deep learning model called "MASK-RCNN" will be use in this case.

Note: this content include only overview/idea of the project. More detail will be provided later.

![RobotArm1](./robot1.gif)

## Requirements
`Hardware`
1. BCN3D Moveo 3D printed robot arm
2. Arduino Mega 2560
3. Dynamixel servo motor (for gripper)

`Language`
1. Python
2. C++

`OS`
1. Ubuntu 18.04+ / Windoow10+

## Overview
![RobotArm1](./robot2.gif)

![DroneCharger](./images/ov2.gif)

To remote control the drone or its base station from far distance, you can remote access to rpi 4 and send keyboard input as control command via VNC server to control the drone, but there will be a bit of latency.

![DroneRpiVNC](./images/ov3.gif)


## Reference
Thank to these following list below, there are useful information and code I've implemented them for this project.
1. [Control Parrot Anafi drone via python coding](https://github.com/Parrot-Developers/olympe)
2. [Control dynamixel servo via python coding](https://github.com/ROBOTIS-GIT/DynamixelSDK)
3. [Control rpi 4 gpio pin via python coding](https://www.ics.com/blog/control-raspberry-pi-gpio-pins-python)
4. [Real VNC Server/Viewer for rpi 4](https://www.realvnc.com/en/connect/download/vnc/raspberrypi/)
