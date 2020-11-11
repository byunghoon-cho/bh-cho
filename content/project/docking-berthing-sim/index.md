---
title: Automated Spacecraft Docking and Berthing
date: "2019-11-08T17:00:00"

authors:
- bh

tags:
- Simulation
- Python
- UR5
- Robotic Arm
- Spacecraft

summary: Simulated the berthing and docking procedure of a spacecraft using the UR5 robotic arm.

image:
    caption: UR5 robotic arm approaching the spacecraft for berthing

    # Focal point (optional)
    # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
    focal_point: Center
---

Docking and berthing are space rendezvous manoeuvres by which two space vehicles become joined.

The docking procedure is achieved when a spacecraft actively moves in a way that it will be able to connect and become attached to another moving vehicle. In this project, the docking performed by the UR5 robotic arm simulated the docking of a spacecraft to the International Space Station (ISS).

On the other hand, berthing is where a robotic arm, such as the Canadarm2, is used to capture a stationary spacecraft and bring it back to a target position. In this project, berthing was performed by using the UR5 robotic arm and the OnRobot RG2 gripper to grab a model spacecraft and guide it towards a set target position.

In both cases, an OpenMV H7 camera was used along with AprilTags to detect the spacecraft.

## Videos
### Berthing
{{< video src="Berthing.mp4" controls="yes" >}}

### Docking
{{< video src="Docking.mp4" controls="yes" >}}
