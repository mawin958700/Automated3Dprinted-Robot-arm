# Automated 3d printed robot arm for Pick & Place
This project is an applying deep learning to robot arm for done some repetitive task extend the charging area for drone landing and control drone and its station from far range via raspberry pi 4. Any device support to qi wireless charging can work as well.

Note: this content include only overview/idea of the project. More detail will be provided later.
## Requirements
`Hardware`
1. Raspberry pi 4
2. Qi charging receiver
3. Qi charger (freedom placement recommended)
4. DC motor (stepper, servo, etc.)

`Software`
1. Real VNC

`OS`
1. Ubuntu 20.10

## Overview
In this project, I use Belkin TrueFreedom PRO as wireless charger attached to dynamixel ax12-a servo motor work together with USB Type C Qi receiver attached to the Parrot Anafi Drone's battery, and the drone power switch need to be able to command on/off button from far distance, so in this case, I use light to trigger power switch by large LDR that you have to make sure there will be no sunlight from ambient environment can trigger the LDR, even though most of drone can't turn off while in flight state. Anyway, LDR is not recommended for outdoor, other passive sensors is more reliable and safety.

![DroneCharger](./images/ov2.gif)

To remote control the drone or its base station from far distance, you can remote access to rpi 4 and send keyboard input as control command via VNC server to control the drone, but there will be a bit of latency.

![DroneRpiVNC](./images/ov3.gif)


## Reference
Thank to these following list below, there are useful information and code I've implemented them for this project.
1. [Control Parrot Anafi drone via python coding](https://github.com/Parrot-Developers/olympe)
2. [Control dynamixel servo via python coding](https://github.com/ROBOTIS-GIT/DynamixelSDK)
3. [Control rpi 4 gpio pin via python coding](https://www.ics.com/blog/control-raspberry-pi-gpio-pins-python)
4. [Real VNC Server/Viewer for rpi 4](https://www.realvnc.com/en/connect/download/vnc/raspberrypi/)
